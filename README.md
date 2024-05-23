class Hero {
    constructor(nome, idade, tipo) {
      this.nome = nome;
      this.idade = idade;
      this.tipo = tipo;
    }
  
    atacar() {
      let ataque;
      switch (this.tipo) {
        case 'mago':
          ataque = 'usou magia';
          break;
        case 'guerreiro':
          ataque = 'usou espada';
          break;
        case 'monge':
          ataque = 'usou artes marciais';
          break;
        case 'ninja':
          ataque = 'usou shuriken';
          break;
        default:
          ataque = 'atacou';
          break;
      }
      console.log(`o ${this.tipo} atacou usando ${ataque}`);
    }
  }
  
  // Exemplo de uso:
  const mago = new Hero('Gandalf', 150, 'mago');
  mago.atacar();  // Saída: "o mago atacou usando magia"
  
  const guerreiro = new Hero('Aragorn', 87, 'guerreiro');
  guerreiro.atacar();  // Saída: "o guerreiro atacou usando espada"
  
  const monge = new Hero('Aang', 12, 'monge');
  monge.atacar();  // Saída: "o monge atacou usando artes marciais"
  
  const ninja = new Hero('Naruto', 17, 'ninja');
  ninja.atacar();  // Saída: "o ninja atacou usando shuriken"
  
