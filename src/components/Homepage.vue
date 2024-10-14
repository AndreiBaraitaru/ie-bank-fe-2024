<template>
  <div class="home-container">
    <header class="home-header">
      <h1>IE Bank Portal</h1>
      <p>Click the button below to manage your accounts!</p>
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
  background: linear-gradient(135deg, #4c74c5, #b0b0b0);
  padding: 20px;
  padding-top:0px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  margin-top: -60px;
}

.home-header h1 {
  font-family: 'Arial', sans-serif;
  font-size: 48px;
  color: white;
  text-shadow: 3px 3px 5px rgba(0, 0, 0, 0.3);
  margin-bottom: 10px;
  text-align: center;
  justify-content: center;
  align-items: center;
}

.home-header p {
  font-size: 24px;
  color: #f0f0f0;
  margin-top: 10px;
  text-shadow: 1px 1px 3px rgba(0, 0, 0, 0.2);
}

.home-content {
  margin-top: 50px;
}

.action-button {
  padding: 15px 30px;
  font-size: 18px;
  background-color: #2b7a78;
  color: white;
  border: none;
  border-radius: 12px;
  cursor: pointer;
  transition: background-color 0.3s, transform 0.2s;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
}

.action-button:hover {
  background-color: #17252A;
  transform: translateY(-2px);
  box-shadow: 0 6px 8px rgba(0, 0, 0, 0.15);
}
</style>

