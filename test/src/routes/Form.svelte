<script lang="ts">
    export function handleName(e: Event, data: any) {
      if ((e.target as HTMLInputElement).value.length > 60) {
          (e.target as HTMLInputElement).value = data.name
      } else {
          data.name = (e.target as HTMLInputElement).value
      }
    }
</script>

<form action="/contact" method="POST" >

    <fieldset>
        <input required id="name" type="text" placeholder='Full Name' maxLength={60}  />
    </fieldset>

    <fieldset>
        <input required id="tel" type="tel" placeholder='Telefone' maxLength={60}  />
    </fieldset>

    <fieldset>
        <input required id="email" type="email" placeholder='E-mail' maxLength={100}  />
    </fieldset>

    <fieldset>
        <select required id="select"  placeholder='Selecione...' >
            <option value="Ninja">Ninja</option>
            <option value="Ninja2">Ninja 2</option>
        </select>
    </fieldset>

    <fieldset>
        <button id="submit" type="submit" value="submit">Quero saber mais!</button>
    </fieldset>

</form>

<style>
     form {
    text-align: center;
    background-color: white;
    color: black;
    padding: 30px 20px;
  }

  fieldset {
    outline: none;
    border:none;
  }

  form button {
    padding: 10px 0px;
    width: 96%;
    border-radius: 10px;
    border: none;

    background-color: var(--green-k);
    transition: background-color .2s ease-in-out;
    color: white;
    
    font-family: "Montserrat", sans-serif;
    font-weight: bold;
    font-size: .9em;

    cursor: pointer;

  }

  form button:hover {
    filter: contrast(80%);
  }

  input, select {
    border: 2px solid #C1BCBC !important;
    border-radius: 10px;
    margin-bottom: 10px;
    background-color: #fff;


    font-family: "Montserrat", sans-serif;
    font-size: .8em;
    color: black;
    
    padding: 10px 0px 10px 10px; 
    width: 95%;
  }
  input:invalid {
    border-color: #900;
    outline: none;
  }

  input:focus:invalid {
    outline: none;
  }
</style>