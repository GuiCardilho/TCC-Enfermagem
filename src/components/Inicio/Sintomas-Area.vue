<template>
  <div class="main-container-sintomasArea" id="Sintomas">
    <div class="container-title-sistomasArea">
      <div class="title-sistomasArea">
        <h1 class="text-title-sintomas">Principais Sintomas</h1>
      </div>
    </div>
    <div class="container-conteudo-sintomas">
      <div class="card-informacao">
        <div class="container-informacao">
          <div class="title-informacao">
            <h1>Sintomas Físicos</h1>
          </div>
          <div class="conteudo-informacao">
            <ul>
              <li>Frequência cardíaca aumentada (coração acelerado)</li>
              <li>Palpitações</li>
              <li>Falta de ar</li>
              <li>Respiração rápida</li>
              <li>Dor ou pressão no peito</li>
              <li>Sensação de asfixia</li>
              <li>Vertigem</li>
              <li>Tontura</li>
              <li>Sudorese</li>
              <li>Calores</li>
              <li>Calafrios</li>
              <li>Náusea</li>
              <li>Estômago embrulhado</li>
              <li>Diarreia</li>
              <li>Tremores</li>
              <li>Estremecimento</li>
              <li>Formigamento ou dormência nos braços ou pernas</li>
              <li>Fraqueza</li>
              <li>Desequilíbrio</li>
              <li>Sensação de desmaio</li>
              <li>Tensão muscular</li>
              <li>Rigidez</li>
              <li>Boca seca</li>
            </ul>
          </div>
        </div>
      </div>

      <div class="card-informacao">
        <div class="container-informacao">
          <div class="title-informacao">
            <h1>Sintomas cognitivos</h1>
          </div>

          <div class="conteudo-informacao">
            <ul>
              <li>Medo de perder o controle</li>
              <li>De ser incapaz de enfrentar</li>
              <li>Medo de dano físico ou de morte</li>
              <li>Medo de “enlouquecer”</li>
              <li>Medo de avaliação negativa dos outros</li>
              <li>Pensamentos</li>
              <li>Imagens ou lembranças assustadoras</li>
              <li>Percepções de irrealidade ou alheamento</li>
              <li>Baixa concentração</li>
              <li>Onfusão</li>
              <li>Distratibilidade</li>
              <li>Estreitamento da atenção</li>
              <li>Hipervigilância para perigo</li>
              <li>Memória fraca</li>
              <li>Dificuldade de raciocínio</li>
              <li>Perda de objetividade</li>
            </ul>
          </div>
        </div>
      </div>

      <div class="card-informacao">
        <div class="container-informacao">
          <div class="title-informacao">
            <h1>Sintomas comportamentais</h1>
          </div>

          <div class="conteudo-informacao">
            <ul>
              <li>Evitação de situações de ameaça</li>
              <li>Fuga</li>
              <li>Busca de segurança</li>
              <li>Agitação</li>
              <li>Andar nervosamente de um lado para outro</li>
              <li>Hiperventilação</li>
              <li>Imobilidade</li>
              <li>Dificuldade para falar</li>
            </ul>
          </div>
        </div>
      </div>

      <div class="card-informacao">
        <div class="container-informacao">
          <div class="title-informacao">
            <h1>Sintomas emocionais</h1>
          </div>

          <div class="conteudo-informacao">
            <ul>
              <li>Sentir-se nervoso</li>
              <li>Tenso</li>
              <li>Irritado</li>
              <li>Assustado</li>
              <li>Aterrorizado</li>
              <li>Apreensivo</li>
              <li>Impaciente</li>
              <li>Frustrado</li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Sintomas-Area",
  components: {},
};
</script>

<style scoped lang="scss">
.main-container-sintomasArea {
  width: 100%;
  min-height: 915px;
  align-items: center;
  justify-content: center;
  border-bottom: 2px solid #089bab;

  background: url("../../assets/circle-scatter-haikei.svg");
  z-index: 0;
  animation: fundo 350s ease-in-out infinite alternate;
  backface-visibility: 30%;
  background-color: rgba(10, 23, 55, 0.5);
}

@keyframes fundo {
  to {
    background-position: 100% 600%;
  }
}

.container-title-sistomasArea {
  padding-top: 10px;
  width: 100%;
  height: 70px;
  display: flex;
  align-items: center;
  justify-content: center;
  background-color: #fff;
  border-bottom: 2px solid #089bab;
  z-index: 1;
}

.title-sintomasArea {
  display: flex;
  text-align: center;
}

.text-title-sintomas {
  font-size: 36px;
  color: #089bab;
}

.container-conteudo-sintomas {
  display: flex;
  flex-direction: column;
  justify-content: center;
  margin-left: 50px;
  align-items: center;
}
.card-informacao {
  height: auto;
  width: 700px;
  display: flex;
  justify-content: center;
  border: 1px solid #7b83eb;
  border-radius: 5px;
  margin: 20px 0px 20px 0px;
  z-index: 1;
  background-color: rgb(255, 255, 255);
  position: relative;
  transition: 0.5s ease;
}

.card-informacao:hover {
  transition: 0.5s ease;
  border: 1px solid #7b83eb;
}

.card-informacao::before {
  content: "";
  width: 50px;
  height: 50px;
  background: url("../../assets/circulo-box-index.svg");
  background-repeat: no-repeat;
  background-size: 80%;
  background-position: 6px 10px;
  position: absolute;
  left: -25px;
  top: -20px;
  border: 1px solid #1c237e;
  border-radius: 50%;
  padding: 5px;
  z-index: 1;
  transition: 0.5s ease;
}

.card-informacao::after {
  content: "";
  width: 50px;
  height: 50px;
  background-color: #fff;
  background-size: 100%;
  background-position: center;
  position: absolute;
  left: -25px;
  top: -20px;
  border: 1px solid #1c237e;
  border-radius: 50%;
  padding: 5px;
  z-index: 0;
  transition: 0.5s ease;
}

.card-informacao:hover::before {
  content: "";
  width: 50px;
  height: 50px;
  background: url("../../assets/circulo-box-index-hover.svg");
  background-repeat: no-repeat;
  background-size: 80%;
  background-position: 6px 10px;
  position: absolute;
  left: -25px;
  top: -20px;
  border: 1px solid #1c237e;
  border-radius: 50%;
  padding: 5px;
  z-index: 1;
  transition: 0.5s ease;
}

.card-informacao:hover::after {
  content: "";
  width: 50px;
  height: 50px;
  background-color: #fff;
  background-size: 100%;
  background-position: center;
  position: absolute;
  left: -25px;
  top: -20px;
  border: 1px solid #1c237e;
  border-radius: 50%;
  padding: 5px;
  z-index: 0;
  transition: 0.5s ease;
}

.container-informacao {
  display: flex;
  flex-direction: column;
  width: 100%;
  height: auto;
  padding: 20px;
}

.title-informacao {
  display: flex;
  justify-content: center;
  align-items: center;
  margin-bottom: 30px;
}

.conteudo-informacao {
  margin-left: 20px;
}

@media (max-width: 750px) {
  .card-informacao {
    width: 500px;
  }
}

@media (max-width: 600px) {
  .card-informacao {
    width: 400px;
  }
}

@media (max-width: 500px) {
  .card-informacao {
    width: 300px;
  }
}
</style>
