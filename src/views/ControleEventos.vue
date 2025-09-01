<template>
  <div class="controle-card">
    <h2>Controle Eventos</h2>
    <div class="controle-content">
      <div class="controle-info">
        <p><strong>Nome do evento:</strong> Pvp no niobio</p>
        <p><strong>Horário:</strong> 21:30</p>
        <p><strong>ID do ganhador:</strong> 2754</p>
        <p><strong>Membros:</strong> 
          <span class="member">@MK</span>
          <span class="member">@Dimas</span>
          <span class="member">@Lucas Rocha</span>
          <span class="member">@Lucas</span>
          <span class="member">@Miguel</span>
          <span class="member">@Raro</span>
          <span class="member">@Twinn</span>
          <span class="member">@aimback</span>
          <span class="member">@miguel fael</span>
          <span class="member">@Sev7en</span>
          <span class="member">@chefao</span>
        </p>
        <p>print: call/jogo</p>
      </div>
      <img src="/controle.png" alt="Controle Evento" />
    </div>
    <p>
      O controle de evento serve para registrar que o evento foi realizado corretamente. Ele deve conter o nome do evento, horário, ID do ganhador, membros presentes e uma print (da call ou do jogo). Esse registro é importante para organização e validação.
    </p>
  </div>
</template>

<script>
export default {
  name: 'ControleEventos'
}
</script>

<style scoped>
.controle-card {
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

.controle-content {
  display: flex;
  gap: 20px;
  align-items: flex-start;
  flex-wrap: wrap;
}

.controle-info {
  flex: 1 1 300px;
  font-size: 1em;
  color: #333;
  line-height: 1.4;
}

.member {
  background: #2f2f2f;
  color: #d1d1d1;
  padding: 4px 8px;
  border-radius: 6px;
  margin-right: 5px;
  font-family: monospace;
  font-size: 0.85em;
  display: inline-block;
  margin-bottom: 5px;
}

.controle-content img {
  max-width: 300px;
  border-radius: 12px;
  box-shadow: 0 4px 10px rgba(0,0,0,0.1);
}

p {
  margin-top: 15px;
}
</style>
