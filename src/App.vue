<template>
  <table class="table">
    <thead>
      <tr>
        <th scope="col">#</th>
        <th scope="col">Nombre</th>
        <th scope="col">Apellido</th>
        <th scope="col">RUT</th>
        <th scope="col">Edad</th>
        <th scope="col">Fecha de Nacimiento</th>
      </tr>
    </thead>
    <tbody>
      <tr v-for="(persona, $index) of personas" :key="$index">
        <td>{{ $index }}</td>
        <td>{{ persona.nombre }}</td>
        <td>{{ persona.apellido }}</td>
        <td>{{ persona.rut }}</td>
        <td>{{ persona.edad }}</td>
        <td>{{ persona.fechaDeNacimiento }}</td>
      </tr>
    </tbody>
  </table>
</template>

<script>


export default {
  name: "App",
  data: () => ({
    personas: [
      {
        nombre: "Belén",
        apellido: "Cid",
        rut: "17.418.625-1",
        edad: 31,
        fechaDeNacimiento: "03-06-1990",
      },
      {
        nombre: "Gonzalo",
        apellido: "Trujillo",
        rut: "16.574.184-6",
        edad: 20,
        fechaDeNacimiento: "12-03-1987",
      },
      {
        nombre: "Facundo",
        apellido: "Braun",
        rut: "15.425.856-k",
        edad: 40,
        fechaDeNacimiento: "01-08-1980",
      },
      
    ],
  }),
};
</script>

<style></style>
