<template>
  <div class="schedule-card">
    <h2><font-awesome-icon icon="clock" /> Horários dos Eventos</h2>
    <table class="schedule-table">
      <thead>
        <tr>
          <th>Hora</th>
          <th>Segunda</th>
          <th>Terça</th>
          <th>Quarta</th>
          <th>Quinta</th>
          <th>Sexta</th>
          <th>Sábado</th>
          <th>Domingo</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="(row, index) in schedule" :key="index">
          <td>{{ row.time }}</td>
          <td>{{ row.monday }}</td>
          <td>{{ row.tuesday }}</td>
          <td>{{ row.wednesday }}</td>
          <td>{{ row.thursday }}</td>
          <td>{{ row.friday }}</td>
          <td>{{ row.saturday }}</td>
          <td>{{ row.sunday }}</td>
        </tr>
      </tbody>
    </table>
    <p class="note">
      Nossos eventos acontecem em dias e horários fixos para que todos possam participar! Todos os horários seguem o fuso de Brasília (BRT).
    </p>
  </div>
</template>

<script>
export default {
  name: 'EventSchedule',
  data() {
    return {
      schedule: [
        { time: '12:30', monday: 'Cante ou Morra', tuesday: 'Fuja da Pantera', wednesday: 'Roleta Russa', thursday: 'Fuja dos Zumbi', friday: 'Vingança dos Players', saturday: 'Ache os Animais', sunday: 'Cante ou Morra' },
        { time: '13:30', monday: 'Briga de Bar', tuesday: 'Todos x Todos', wednesday: 'Briga de Rua', thursday: 'Taco x Taco', friday: 'Desce e Quebra de Moto', saturday: 'Desce e Quebra', sunday: 'Desce e Quebra' },
        { time: '14:30', monday: 'Panto x Rampa', tuesday: 'Corrida de Kart', wednesday: 'Among-Us', thursday: 'Corrida de Jetskin', friday: 'Corrida de Bike', saturday: 'Fuja da Pantera', sunday: 'Panto x Rampa' },
        { time: '16:30', monday: 'Todos x Todos', tuesday: 'Pvp no Labirinto', wednesday: 'X1 no Rolas', thursday: 'Mini Royale', friday: 'Pvp de Sniper (Zancudo)', saturday: 'Pvp no CS', sunday: 'Pvp Paleto' },
        { time: '18:30', monday: 'Tacada Mortal', tuesday: 'Esconde Esconde', wednesday: 'Caminhão Bolado', thursday: 'Fuja Bicudo', friday: 'Panto x Rampa', saturday: 'Proteja a Juiza', sunday: 'Resgate o Comando Geral' },
        { time: '20:30', monday: 'Corrida de Moto', tuesday: 'Pvp de Marchado', wednesday: 'Corrida Maluca', thursday: 'Baile do Muro', friday: 'Desce e Quebra de Blindado', saturday: 'Dominas Paleto', sunday: 'Dominas Porto' },
        { time: '22:30', monday: 'Fuja do Neymar', tuesday: 'Fuja do Macaco', wednesday: 'Pvp na Construção', thursday: 'Pvp no BC', friday: 'Ataque x Defesa', saturday: 'Corrida de Moto', sunday: 'Corrida de Avião' },
        { time: '23:30', monday: 'Battle Royale', tuesday: 'Battle Royale', wednesday: 'Battle Royale', thursday: 'Battle Royale', friday: 'Battle Royale', saturday: 'Battle Royale', sunday: 'Battle Royale' }
      ]
    }
  }
}
</script>

<style scoped>
.schedule-card {
  background: white;
  border-radius: 12px;
  box-shadow: 0 6px 15px rgba(0,0,0,0.1);
  padding: 20px;
  margin-top: 20px;
}

h2 {
  color: #6b21a8;
  margin-bottom: 15px;
  font-weight: 700;
  font-size: 1.8em;
  display: flex;
  align-items: center;
  gap: 10px;
}

.schedule-table {
  width: 100%;
  border-collapse: collapse;
  text-align: center;
  font-size: 1em;
}

.schedule-table th,
.schedule-table td {
  border: 1px solid #ddd;
  padding: 10px;
}

.schedule-table th {
  background-color: #5a2d82;
  color: white;
  font-weight: 600;
}

.schedule-table tbody tr:nth-child(even) {
  background-color: #f9f9f9;
}

.note {
  margin-top: 15px;
  font-size: 1em;
  color: #333;
  font-style: italic;
}
</style>
