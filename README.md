# Scan IP

> Pega o IP externo e também verifica se a porta do seu servidor está aberta ou não.

**Tecnologias Utilizadas**

- ReactJS (Cliente)
- NodeJS (Servidor)


> Há vários sites que fazem isso, então porquê criar este?

Eu particularmente ligo muito pra o visual do site, e praticamente todos os websites que oferecem isso, tem um visual antigo. Então eu resolvi dar uma renovada no visual, e fazer o website virar instalável (assim você pode utilizar sempre, em qualquer lugar)


> Hospedagem e Servidor

- Vercel (Utilizei o Vercel para armazenar o front-end)
- Heroku (Utilizei o Heroku para armazenar o back-end)

***GIF***

![Peek 2020-09-13 12-09](https://user-images.githubusercontent.com/40338524/93024486-47cdec80-f5cd-11ea-934d-7b371e382fed.gif)

**Demonstração**

[Site "Teste de Portas"](http://teste-porta.vercel.app/)

---

## Principais bibliotecas utilizadas

- Styled-Components
- Axios
- Express

---

## Recuperando o IP Externo

```javascript
async index(req, res) {
    const ip = req.headers['x-forwarded-for']
    await res.status(200).json({
            ip: ip,
    });
}
```

---

### Clone

- Clone this repo to your local machine using `https://github.com/kingaspx/Scanner-Net.git`

> Instalando o Servidor

```shell
$ cd server
$ yarn install
```

> Instalando o Cliente

```shell
$ cd client
$ yarn install
```

## Team

> O cara mais lindo do mundo (diga-se de passagem)

| <a href="http://youtube.com/c/kingaspx" target="_blank">**Abner Rodrigues**</a> |
| :---: |
| [![Abner](https://user-images.githubusercontent.com/40338524/93024738-edce2680-f5ce-11ea-9794-5011cf659bab.png)]|

---

## Support

Reach out to me at one of the following places!

- Facebook at <a href="http://instagram.com/kingaspx" target="_blank">`@rodriguesabner_`</a>
- Instagram at <a href="http://instagram.com/rodriguesabner_" target="_blank">`@kingaspx`</a>
- Youtube at <a href="http://youtube.com/c/kingaspx" target="_blank">`@kingaspx`</a>

---

## Donations (Optional)
[![Support via Patreon](https://cloakandmeeple.files.wordpress.com/2017/06/become_a_patron_button3x.png?w=200)](https://www.patreon.com/bePatron?u=42288653)

---