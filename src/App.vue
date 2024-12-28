<template>
  <div class="app">
    <nav class="navbar">
      <div class="nav-brand">CryptoInfo</div>
      <div class="nav-links">
        <router-link to="/" class="nav-link">Home</router-link>
        <router-link to="/discussion" class="nav-link">Discussion</router-link>
        <router-link to="/exchange" class="nav-link">Exchange</router-link>
        <router-link to="/contact" class="nav-link">Contact Me</router-link>
      </div>
    </nav>

    <main class="main-content">
      <router-view></router-view>
    </main>

    <footer class="footer">
      <div class="footer-content">
        <p>Contact: your.email@example.com</p>
        <p>&copy; 2024 CryptoInfo. All rights reserved.</p>
      </div>
    </footer>
  </div>
</template>

<style>
.app {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
}

.navbar {
  background-color: #2c3e50;
  padding: 1rem 2rem;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.nav-brand {
  color: white;
  font-size: 1.5rem;
  font-weight: bold;
}

.nav-links {
  display: flex;
  gap: 2rem;
}

.nav-link {
  color: white;
  text-decoration: none;
  padding: 0.5rem 1rem;
  border-radius: 4px;
  transition: background-color 0.3s;
}

.nav-link:hover {
  background-color: #34495e;
}

.main-content {
  flex: 1;
  padding: 2rem;
}

.footer {
  background-color: #2c3e50;
  color: white;
  padding: 1rem;
  text-align: center;
}

.footer-content {
  max-width: 1200px;
  margin: 0 auto;
}
</style>