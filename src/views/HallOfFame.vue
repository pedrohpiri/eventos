<template>
  <div class="halloffame-card">
    <h2>Registro Hall-Fama</h2>
    <div class="halloffame-content">
      <img src="/halldafalam.png" alt="Hall da Fama" />
      <div class="halloffame-text">
        <h3>Grande Vencedor</h3>
        <p>
          O Hall da Fama é o registro oficial de todos os eventos que realizamos. Nele ficam armazenados os resultados, participantes e detalhes importantes, servindo como histórico para consulta e organização da equipe.
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HallOfFame'
}
</script>

<style scoped>
.halloffame-card {
  background: white;
  border-radius: 12px;
  box-shadow: 0 6px 15px rgba(0,0,0,0.1);
  padding: 20px;
  margin-top: 20px;
}

h2 {
  color: #6b21a8;
  margin-bottom: 15px;
}

.halloffame-content {
  display: flex;
  gap: 20px;
  align-items: center;
}

.halloffame-content img {
  max-width: 300px;
  border-radius: 12px;
  box-shadow: 0 4px 10px rgba(0,0,0,0.1);
}

.halloffame-text h3 {
  color: #ffcc00;
  margin-bottom: 10px;
  font-weight: 700;
  text-shadow: 0 0 5px #ffcc00;
}

.halloffame-text p {
  font-size: 1em;
  color: #333;
  line-height: 1.4;
}
</style>
