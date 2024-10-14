<template>
  <div class="home-container">
    <header class="home-header">
      <h1>IE Bank Portal</h1>
      <p>Your gateway to better financial management.</p>
    </header>
    <main class="home-content">
      <button class="action-button" @click="goToAccounts">Manage Accounts</button>
    </main>
  </div>
</template>

<script>
export default {
  name: 'HomePage',
  methods: {
    goToAccounts() {
      
      this.$router.push({ path: '/accounts' });
    }
  }
};
</script>

<style scoped>
.home-container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  height: 100vh;
  background: linear-gradient(to right, #5A7D7C, #B0D6D6);
}

.home-header h1 {
  font-family: 'Arial', sans-serif;
  font-size: 48px;
  color: white;
  text-shadow: 2px 2px #333;
}

.home-header p {
  font-size: 24px;
  color: #333;
  margin-top: 10px;
}

.home-content {
  margin-top: 40px;
}

.action-button {
  padding: 15px 30px;
  font-size: 18px;
  background-color: #2b7a78;
  color: white;
  border: none;
  border-radius: 8px;
  cursor: pointer;
  transition: background-color 0.3s;
}

.action-button:hover {
  background-color: #17252A;
}
</style>
