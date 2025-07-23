<template>
  <div class="dashboard">
    <h1>Welcome, {{ studentName }} 👋</h1>
    <p>Your personalized Student Dashboard is ready!</p>

    <div class="info">
      <p>Here’s what you can do:</p>
      <ul>
        <li>✅ Check your assignments</li>
        <li>📚 View learning resources</li>
        <li>📅 Track your attendance</li>
        <li>📝 Take quizzes and view results</li>
      </ul>
    </div>

    <div class="links">
      <h3>Quick Links</h3>
      <ul>
        <li><a href="#">My Assignments</a></li>
        <li><a href="#">Lecture Notes</a></li>
        <li><a href="#">Quiz Portal</a></li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    studentName: {
      type: String,
      default: 'Student'
    }
  }
}
</script>

<style scoped>
.dashboard {
  max-width: 600px;
  margin: 50px auto;
  text-align: center;
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  padding: 20px;
  border: 2px solid #ccc;
  border-radius: 12px;
  background-color: #f9f9f9;
}

.info ul {
  list-style: none;
  padding: 0;
}

.info li {
  margin: 8px 0;
  font-size: 16px;
}

.links ul {
  list-style-type: none;
  padding: 0;
}

.links a {
  color: #2c3e50;
  text-decoration: none;
  font-weight: bold;
}

.links a:hover {
  text-decoration: underline;
}
</style>
