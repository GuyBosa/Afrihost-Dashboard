<template>
  <div>
    <h1>Contact Me</h1>
  <p>
    <ul>
      <li>Email: {{email}}</li>
      <li>LinkedIn: {{linkedIn}}</li>
    </ul>
  </p>
  </div>
</template>

<script>
export default {
  name: 'Contact',
  data () {
    return {
      email: 'guybosa0@gmail.com',
      linkedIn: 'https://www.linkedin.com/in/guy-bosa/'
    }
  }
}
</script>
