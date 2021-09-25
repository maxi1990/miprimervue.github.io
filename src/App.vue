<template>
  <div class="container">
        <h1 class="text-center p-5">Tabla de Usuarios</h1>
      <table class="table table-striped" id="table">
        <thead>
          <tr>
            <th scope="col">#</th>
            <th scope="col">Nombre</th>
            <th scope="col">Apellido</th>
            <th scope="col">RUN</th>
            <th scope="col">Fecha de nacimiento</th>
            <th scope="col">Edad</th>
          </tr>
        </thead>
        <tbody>
          <tr v-for="(persona, index) in personas" :key="index">
            <th scope="row">{{persona.id}}</th>
            <td>{{persona.nombre}}</td>
            <td>{{persona.apellido}}</td>
            <td>{{persona.run}}</td>
            <td>{{persona.fechaNacimiento}}</td>
            <td>{{persona.edad}}</td>
          </tr>
        </tbody>
      </table>
    </div>
</template>

<script>
export default {
  name: 'App',
  data: () => ({
    personas: [{
      id: 1,
      nombre: "Maximiliano",
      apellido: "Gutierrez",
      run: "17.562.117-2",
      fechaNacimiento: "07-01-1990",
      edad: "31"
    },
    {
      id: 2,
      nombre: "Maria",
      apellido: "Campos",
      run: "16.642.353-3",
      fechaNacimiento: "25-04-1988",
      edad: "33"
    },
    {
      id: 3,
      nombre: "Erika",
      apellido: "Cerda",
      run: "18.368.569-2",
      fechaNacimiento: "10-06-1992",
      edad: "29"
    }]
  })
}
</script>

<style>
</style>
