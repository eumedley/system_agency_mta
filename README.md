# 🚀 Sistema de Empregos (MTA:SA)

Sistema completo de empregos para servidores MTA:SA, com interface moderna, persistência em banco de dados e estrutura organizada para fácil manutenção e expansão.

---

## 📌 Funcionalidades

* ✔ Sistema de agência de empregos com UI customizada
* ✔ Seleção de empregos com requisitos de level
* ✔ Persistência de emprego (SQLite)
* ✔ Integração com elementData (configurável)
* ✔ Sistema de scroll para múltiplos empregos
* ✔ Validação server-side (anti exploit)
* ✔ Sistema de infobox (client/server)
* ✔ Código modular e organizado

---

## ⚙️ Configuração

Toda a configuração do sistema é feita no arquivo:

```
Config.lua
```

### 🔧 ElementData

```lua
DATAS = {
    level = "player:level",
    job = "player:job",
}
```

---

### 🏢 Agência

```lua
AGENCY = {
    {x, y, z, tipo, tamanho, r, g, b, alpha}
}
```

---

### 💼 Jobs

Cada job possui:

```lua
{
    name = "Nome",
    level = 0,
    salary = 10000,
    location = {x, y, z},
    description = "Descrição",
    image = "caminho.png",
    data = "ID interno"
}
```

---

## 🎮 Como usar

1. Vá até uma agência no mapa
2. Escolha um emprego disponível
3. Clique em **Trabalhar**
4. Use `/infos` para marcar o local do trabalho

---

## 🧠 Estrutura

* `client.lua` → Interface e interação do jogador
* `server.lua` → Lógica, validação e banco de dados
* `config.lua` → Configuração geral do sistema

---

## 🔒 Segurança

* Validação completa no server
* Anti spam de eventos

---

## 🚧 Possíveis melhorias

* Sistema de XP por emprego
* Waypoint automático
* Cooldown para troca de emprego
* Missões específicas por job
* Sistema de progressão

---

## 👨‍💻 Autor

Desenvolvido por **Medley** (#medleyon)

---

## 📄 Licença

Uso livre para projetos pessoais/comerciais.
Créditos são apreciados
