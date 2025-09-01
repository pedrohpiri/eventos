<template>
  <div class="commands-card">
    <h2>Comandos de Eventos</h2>
    <div class="commands-content">
      <pre class="commands-list">
Events (PUXAR F3)
ADM (SOLTAR AVISO)
CAR NOMEDOCARRO (SPAWNAR CARRO)
SKIN ID NOMEDASKIN (SETAR SKIN)
SETPRESET ID (SEU) ID (DA PESSOA)....(SETA SEU PRESET NA PESSOA)
MUNDOAREA MUNDO 10 (TODOS NO RAIO DE METROS DO NUMERO VAI PARA O MUNDO)
god id pp (MANDA A PESSOA PARA O PIER NO MUNDO PADRÃO)
GODAREA 50 - METROS (DA GOD EM TODO MUNDO NA AREA DE 50 METROS ETC)
NC - (FICA INVISIVEL E PODE VOAR NA CIDADE)
TPTO ID - (TELEPORTA ATE A PESSOA)
TPTOME ID - (PUXA A PESSOA ATE O LOCAL ONDE VOCE ESTA)
TPWAY (TELEPORTA VOCE ATE O LOCAL MARCADO NO SEU MAPA)
WALL (ATIVA AS INFORMAÇÕES DOS PLAYERS)
DV (APAGA OS VEICULOS)
FIX (CONCERTA OS VEICULOS)
som (radio para meter musica)
e3 dancar2 20 (e3 serve pra colocar todos para dançar)
      </pre>
      <p>
        Os comandos de eventos servem para organizar e controlar tudo durante a realização de um evento. São utilizados para puxar membros, iniciar, encerrar, dar avisos ou padronizar roupas. Apenas quem tem autorização pode usá-los.
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Commands'
}
</script>

<style scoped>
h2 {
  color: #6b21a8;
  margin-bottom: 15px;
}
pre {
  background-color: #1e1e1e;
  color: #d4d4d4;
  padding: 15px;
  border-radius: 8px;
  overflow-x: auto;
  font-family: 'Courier New', Courier, monospace;
  white-space: pre-wrap;
  flex: 1 1 300px;
  max-width: 600px;
  box-shadow: 0 4px 10px rgba(0,0,0,0.1);
}

.commands-card {
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

.commands-content {
  display: flex;
  gap: 20px;
  align-items: flex-start;
  flex-wrap: wrap;
}

.commands-content p {
  flex: 1 1 300px;
  font-size: 1em;
  color: #333;
  line-height: 1.4;
  margin: 0;
}
</style>
