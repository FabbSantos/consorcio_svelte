<script>
	import KawaLogo  from '$lib/images/logo_kawsaki-2.webp';
</script>

    <header>
      <div class="logo">
        <a href="/" target="_blank">
          <img src={ KawaLogo } alt="Kawasaki Logo">
        </a>
      </div>
      <ul>
        <li>
          <a href="/" target="_blank">
            Home
          </a>
        </li>
        <li>
          <a href="/" target="_blank">
            Quem Somos
          </a>
        </li>
        <li>
          <a href="/" target="_blank">
            Como Funciona
          </a>
        </li>
        <li>
          <a href="/" target="_blank">
            <button class="sim">Faça uma Simulação</button> 
          </a>
        </li>
      </ul>
    </header>

<style>
	header {
  display: flex;
  background: #000;
}

header .logo a {
  display: inline-block;
  padding: 10px 10px 7px 20px;
}
header .logo {
  margin-left: 12em;
}
@media (max-width: 768px){
  header .logo {
    margin-left: 0;
  }
}

header ul {
  margin: 0 auto;
  max-width: 70vw; 
  padding: 3px 10px 0 0;
  list-style: none;
  flex: 1;
  text-align: right;
}

header li {
  display: inline-block;
  margin: 0;
  padding: 0;
}

header li a {
  display: inline-block;
  color: #fff ;
  padding: 15px 10px;
  text-decoration: none;
}

header li a:hover {
  text-decoration: underline;
}
header li a button {
  color: inherit;
  font-size: inherit;
  font-family: inherit;

  outline: none;
  background-color: transparent;
  border: 1px solid #fff;

  cursor: pointer;
  padding: 6px 20px;
  border-radius: 1em;

  transition: 0.3s ease;
}
header li a button:hover {
  background-color: white;
  color: black;  
}
</style>
