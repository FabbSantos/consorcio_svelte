<script>
	// @ts-ignore
	import FaCoins from 'svelte-icons/fa/FaCoins.svelte';
	// @ts-ignore
	import FaPhone from 'svelte-icons/fa/FaPhone.svelte';
	import Form from './Form.svelte';
</script>

<div class="outside bg">
	<div class="container">
		<div class="t-row">
			<div class="left-box">
				<div class="text">
					<h2><b>CONSÓRCIO KAWASAKI BRASIL</b></h2>
					<h1><b>LIBERTE</b> SEU <b>SONHO</b> DE TER UMA <b>MOTO!</b></h1>
				</div>

				<div class="rows">
					<div class="f-row">
						<div>
							<h2>SEM <br /><i>JUROS</i></h2>
						</div>
						<div>
							<h2>SEM <br /><i>ENTRADA</i></h2>
						</div>
					</div>
					<div class="s-row">
						<div><h2>PLANOS DE ATÉ <br /><i>100 MESES</i></h2></div>
					</div>
				</div>
			</div>
			<div class="right-box">
				<h2>Deixe suas informações e conheça os <b>planos e vantagens!</b></h2>
				<Form />
			</div>
		</div>

		<div class="b-row">
			<div class="carac">
				<div>
					<span>
						<FaPhone class="icon" />
					</span>
					<h3>
						Atendimento<br />
						<span>(16) 2103-3536</span>
					</h3>
				</div>
				<div>
					<span><FaCoins class="icon" /></span>
					<h3>Vendas<br /><span>0800 943 3500</span></h3>
				</div>
				<div>
					<span><FaPhone class="icon" /></span>
					<h3>WhatsApp Atendimento<br /><span>(16) 2103-3535</span></h3>
				</div>
				<div>
					<span><FaPhone class="icon" /></span>
					<h3>WhatsApp Vendas<br /><span>(16) 2103-3501</span></h3>
				</div>
			</div>
		</div>
	</div>
</div>

<style>.bg {
  background-image: url("assets/img/bg-moto.webp" );
  background-repeat: no-repeat;
  background-size: cover;
}
.outside {
  width: 100%;
  min-height: 90vh;
}

body > main > section > div.outside.bg > div > div.t-row > div.left-box > div.text {
    text-align: left;
}
.t-row {
    display: flex;
    width: 100%;
    align-items: center;
    gap: 10em;
    justify-content: space-around;
}
.left-box {
  width: 50%; 
  padding: 50px;
}
.left-box h2{
    font-size: 1.3em;
}
.left-box h1 {
    font-size: 2.5em;
}
.rows {
    display: flex;
    width: 100%;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    gap: 1.2em;
}
.f-row, .s-row{
    width: 100%;
}
.f-row, .left-box{
    gap: 1.2em;
}
.left-box .f-row, .left-box .f-row div, .left-box .s-row{
    display: flex;
    justify-content: center;
    align-items: center;
}
.left-box .f-row div, .left-box .s-row div {
    width: 50%;
    text-align: center;
    padding: 5px 0;
    background-color: var(--green-k);
}
.left-box .f-row div:first-child {
    border-radius: 30px 5px 5px 5px;
}
.left-box .f-row div:last-child {
    border-radius: 5px 5px 30px 5px;
}
.left-box .s-row div{
    width: 100%;
    border-radius: 30px 5px 30px 5px;
    padding: 5px 20px; 
}

.left-box .f-row h2, .left-box .s-row h2{
    font-weight: 600;
    font-size: 1.5em;
}
.left-box .f-row h2 i{
    font-weight: 700;
    font-size: 1.3em;
}
.left-box .s-row h2 i{
    font-weight: 700;
    font-size: 2em;
}

.text {
    margin-bottom: 4em;
}
.right-box {
    width: 40%;
}
.right-box h2{
    font-size: 1.3em;
    text-align: center;
}

.b-row {
    width: 100%;
    display: flex;
    justify-content: baseline;
    align-items: center;
}

.carac {
    border-radius: 85px;
    width: 100%;
    padding: 15px;
    background-color: var(--green-k);
    
    display: flex;
    flex-direction: row;
    justify-content: space-around;
    align-items: center;
}
.icon {
    height: 30px;
    stroke-width: 1.5;
}
.carac div{
    display: flex;
    gap: .9em;
    flex-direction: row;
    align-items: center;
    justify-content: center;
}
.carac div h3{
    font-size: 1em;
    text-transform: uppercase;
}
.carac div h3 span{
    text-decoration: underline;
    cursor: pointer;
}

@media (max-width: 768px) {
    .outside {
        height: auto;
    }
    .t-row {
        gap: 2em;
        padding-top: 40px;
        flex-direction: column-reverse;
        text-align: center;
    }
    .left-box {
        padding: 1em 0px;
    }
    .left-box, .right-box {
        width: 100%;
    }
    .rows {
        font-size: 0.8em;
    }
    .carac {
        border-radius: 30px 5px 30px 5px;
        flex-direction: column;
        gap: 2em;
        margin-bottom: 2em;
    }
    .carac div {
        width: 100%;
        gap: .5em;
        flex-direction: column;
        text-align: center;
    }
}
</style>
