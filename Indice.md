# HTML

*Hypertext*

*Markup*
- Tag
- Atributos

*Language*

# CSS
Cascading StyleSheet

```css
/* declarações */
body {
    background-color: black;
    color: white;
}
```

# JavaScript
```js
// variaveis
const mensagem = 'oi, tudo bem?'
// tipos de dados
    // number
    // string
// funçao
alert(mensagem)

// obejto javascript
const participante = {
    nome: "Breno Miranda",
    email: "brenomiranda000@gmail.com",
    dataInscricao: new Date(2024, 2, 22, 19, 20),
    dataCheckIn: new Date(2024, 2, 25, 22, 0)
}

// array
let participantes = [
    {
        nome: "Breno Miranda",
        email: "brenomiranda000@gmail.com",
        dataInscricao: new Date(2024, 2, 22, 19, 20),
        dataCheckIn: new Date(2024, 2, 25, 22, 0)
    },
]

// estrutura de repetição - loop
for(let participante of participantes) {
    // faça alguma coisa aqui
    // enquanto tiver participantes nessa lista
    output = output + criarNovoParticipante(participante)
}

// Condicional
    if(participante.dataCheckIn == null) {
        dataCheckIn = `
            <button
                data-email="${participante.email}"
                onclick="fazerCheckIn(event)"
            >
                confirmar check-in
            </button>
        `
    }

// verificar se o participante já existe 1
    const participanteExiste = participantes.find(
        (p) => {
          return p.email == participante.email
        }
    )

    if(participanteExiste) {
        alert('Participante já cadastrado!')
        return
    }

// verificar se o participante já existe 2
// ele retorna altomaticamente, questão mais visual 
    const participanteExiste = participantes.find(
        (p) => p.email == participante.email
    )

    if(participanteExiste) {
        alert('Participante já cadastrado!')
        return
    }

```