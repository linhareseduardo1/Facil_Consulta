<template>
  <div class="hello">
    <div class="container">
      <div class="row">
        <div class="col-md-6 rounded px-5 py-4 shadow bg-white text-left">
          <h1>Sobre o profissional</h1>
          <h2>Dados do profissional</h2>
          <div id="header"></div>
          <form id="home" @submit="checkForm" action="#" method="post">
            <!--
    <p v-if="errors.length">
      <b>Por favor, corrija o(s) seguinte(s) erro(s):</b>
      <ul>
        <li v-for="error in errors">{{ error }}</li>
      </ul>
    </div> -->
            <div class="form-group">
              <label for="name">Nome completo* </label>
              <br />
              <input
                id="name"
                v-model="name"
                class="form-control"
                type="text"
                name="name"
                placeholder="Digite o nome completo"
              />
            </div>

            <div class="form-group">
              <label for="age">CPF* </label><br />
              <input
                id="cpf"
                v-model="cpf"
                class="form-control"
                type="cpf"
                name="cpf"
                min="9"
                max="9"
                placeholder="Digite um CPF"
              />
            </div>

            <div class="form-group">
              <label for="tel">Número de celular* </label><br />
              <input
                id="tel"
                v-model="phone"
                class="form-control"
                type="cpf"
                name="cpf"
                min="9"
                max="9"
                placeholder="(00) 0 0000-0000"
              />
            </div>
            <div class="form-group">
              <label for="estado">Estado* </label><br />
              <select
                id="estado"
                v-model="estado"
                class="form-control"
                name="estado"
              >
                <option>Paraná</option>
                <option>Rio Grande do Sul</option>
                <option>Santa Catarina</option>
              </select>
            </div>
            <div class="form-group">
              <label for="cidade">Cidade* </label><br />
              <select
                id="cidade"
                v-model="cidade"
                class="form-control"
                name="estado"
              >
                <option>Londrina(PR)</option>
                <option>Maringá(PR)</option>
                <option>Pelotas(RS)</option>
                <option>Porto Alegre(RS)</option>
                <option>Florianópolis(SC)</option>
                <option>Joinville (RS-)</option>
              </select>
            </div>
            <br />
            <div class="form-group">
              <input type="submit" class="form-control" value="PRÓXIMO" />
            </div>
          </form>
        </div>
        <div class="imagem vue-bg col-md-4 d-flex align-items-center">
          <img alt="Vue logo" src="../assets/desktop-pagina-1.png" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default { name: "PageHome" };
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss">
$primary-0: #483698;

h1 {
  color: $primary-0;
  font-family: Verdana, Geneva, Tahoma, sans-serif;
}
</style>


<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
