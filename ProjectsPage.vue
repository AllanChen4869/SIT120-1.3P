<template>
    <div>
      <h1>My Projects</h1>
      <table>
        <thead>
          <tr>
            <th>Project Name</th>
            <th>Description</th>
          </tr>
        </thead>
        <tbody>
          <tr v-for="project in projects" :key="project.id">
            <td>{{ 'Game Hub' }}</td>
            <td>{{ 'GameHub is a comprehensive online platform dedicated to gaming enthusiasts, where they can discover, purchase, and interact with their favorite games and connect with fellow gamers. The platform aims to provide an immersive gaming experience, focusing on user engagement, community building, and accessibility' }}</td>
          </tr>
        </tbody>
      </table>
    </div>
  </template>
<script>
export default {
  data() {
    return {
      projects: [
        { id: 1, name: 'Project 1', description: 'Description for project 1' },
        // ... add your other projects here
      ]
    };
  }
};
</script>
<style>
table {
  width: 100%;
  border-collapse: collapse;
  margin-top: 20px;
}

table, th, td {
  border: 1px solid #e0e0e0;
}

th, td {
  padding: 10px 15px;
  text-align: left;
}

th {
  background-color: #f5f5f5;
  color: #555;
}

tr:hover {
  background-color: #f9f9f9;
}

</style>  