<template>
  <div class="staff-info-card">
    <h2><font-awesome-icon icon="mask" /> Máscara Oficial da Pasta</h2>
    <div class="mask-content">
      <img src="/mascara.png" alt="Máscara Oficial" />
      <div class="mask-details">
        <ul>
          <li><strong>Máscara:</strong> 238</li>
          <li><strong>Textura:</strong> 5</li>
        </ul>
        <p>Todos os membros devem utilizá-la conforme o padrão estabelecido.</p>
      </div>
    </div>
    <h3>Hierarquia dos Eventos</h3>
    <div class="hierarquia-container">
      <ul>
        <li><font-awesome-icon icon="star" class="icon adm-icon" /><span class="role adm">ADM</span> <span class="mention">@MK</span></li>
        <li><font-awesome-icon icon="shield-alt" class="icon responsavel-icon" /><span class="role responsavel">Responsável EvT</span> <span class="mention">@Resp EvT | Thigas</span> <span class="mention">@Resp EvT | Gabiss</span></li>
        <li><font-awesome-icon icon="user-shield" class="icon auxiliar-icon" /><span class="role auxiliar">Auxiliar EvT</span> <span class="mention">@Aux. EvT | Zack Cross</span> <span class="mention">@Aux. EvT | Barleta | 3149</span></li>
        <li><font-awesome-icon icon="rocket" class="icon lider-icon" /><span class="role lider">Líder EvT</span> <span class="mention">@Lid. EvT | Sev7en</span> <span class="mention">@Lid. EvT | Lucas Ribeiro</span></li>
        <li><font-awesome-icon icon="user-tie" class="icon sublider-icon" /><span class="role sublider">Sub-Líder EvT</span> <span class="mention">@Sub. EvT | chefao</span> <span class="mention">@Sub. EvT | Raro | 1047</span></li>
      </ul>
      <p>
        A hierarquia deve ser sempre respeitada nos eventos. Qualquer problema que envolva membros teste ou membros deve ser reportado primeiro ao sub-líder de eventos. Caso ele não consiga resolver ou não esteja presente, o próximo passo é procurar o líder. Se ainda assim não houver solução, deve-se recorrer ao AUX ou ao responsável da pasta de eventos. É <strong>estritamente proibido</strong> entrar em contato direto com o ADM da pasta, <strong>exceto em casos extremos</strong>. Seguir essa ordem garante organização e respeito entre todos.
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'StaffInfo'
}
</script>

<style scoped>
.staff-info-card {
  background: white;
  border-radius: 12px;
  box-shadow: 0 6px 15px rgba(0,0,0,0.1);
  padding: 20px;
  margin-top: 20px;
}

h2 {
  color: #6b21a8;
  margin-bottom: 15px;
  display: flex;
  align-items: center;
  gap: 10px;
}

.mask-content {
  display: flex;
  gap: 20px;
  align-items: center;
  margin-bottom: 20px;
}

.mask-content img {
  max-width: 300px;
  border-radius: 8px;
  box-shadow: 0 4px 10px rgba(0,0,0,0.1);
}

.mask-details ul {
  list-style: none;
  padding: 0;
  margin: 0 0 10px 0;
}

.mask-details li {
  font-weight: bold;
  margin-bottom: 5px;
}

.mask-details p {
  font-weight: normal;
  color: #444;
}

h3 {
  margin-top: 30px;
  color: #5a2d82;
}
.hierarquia-container {
  background: #1a1a1a;
  color: white;
  padding: 20px;
  border-radius: 12px;
  margin-top: 20px;
  box-shadow: 0 6px 15px rgba(0,0,0,0.2);
}

.hierarquia-container ul {
  list-style: none;
  padding: 0;
  margin: 0 0 15px 0;
}

.hierarquia-container li {
  margin-bottom: 10px;
  font-weight: 600;
  display: flex;
  align-items: center;
  gap: 10px;
}

.role {
  padding: 4px 8px;
  border-radius: 6px;
  font-size: 0.9em;
  font-weight: 700;
  color: white;
}

.adm {
  background: #ff4500;
}

.responsavel {
  background: #ffa500;
}

.auxiliar {
  background: #32cd32;
}

.lider {
  background: #1e90ff;
}

.sublider {
  background: #9370db;
}

.mention {
  background: #2f2f2f;
  padding: 4px 8px;
  border-radius: 6px;
  font-family: monospace;
  font-size: 0.85em;
  color: #d1d1d1;
}
.icon {
  margin-right: 8px;
  color: #ffd700;
}

.adm-icon {
  color: #ff4500;
}

.responsavel-icon {
  color: #ffa500;
}

.auxiliar-icon {
  color: #32cd32;
}

.lider-icon {
  color: #1e90ff;
}

.sublider-icon {
  color: #9370db;
}
</style>
