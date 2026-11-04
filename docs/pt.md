# Jaya Player — guia de utilização

O Jaya Player é um leitor IPTV para Android TV, TV boxes e smartphones.
A aplicação **não fornece canais de TV nem conteúdo**: reproduz apenas as listas que o próprio utilizador adiciona.

---

## 1. Instalação

1. Descarregue a aplicação: **https://github.com/FirstRandomUser/jaya-player-releases/releases/latest/download/jaya-player.apk** (sempre a versão mais recente) ou na página [Releases](https://github.com/FirstRandomUser/jaya-player-releases/releases/latest).
2. Numa TV box é prático usar a aplicação **Downloader** ou uma pen USB.
3. Na primeira instalação, o Android pede para permitir instalações desta origem — permita.
4. É necessário o Android 6.0 ou mais recente.

Depois disso, a aplicação descarrega e instala as atualizações **sozinha** (ver secção 10).

---

## 2. Primeiro arranque e lista

No primeiro arranque abrem-se as **Definições**.

1. Prima **Listas → Adicionar**.
2. Escolha o tipo:
   - **ligação M3U** — endereço da lista do seu fornecedor;
   - **Xtream Codes** — endereço do servidor, utilizador e palavra-passe;
   - **ficheiro** — lista `.m3u` do dispositivo ou de uma pen USB.
3. **EPG** (guia de programação) — endereço XMLTV. Normalmente já vem na lista do fornecedor e o campo pode ficar vazio. Se não houver guia, peça o endereço EPG ao seu fornecedor e escreva-o aqui.
4. **Atualizar a cada … h** — com que frequência atualizar a lista e o guia.
5. Prima **Guardar**. O carregamento corre em segundo plano — pode voltar logo a ver TV.

Pode adicionar várias listas. Se uma atualização falhar (por exemplo, sem internet), a aplicação repete-a sozinha no próximo arranque.

---

## 3. Comando

| Botão | Ação |
|---|---|
| ▲ ▼ | canal anterior / seguinte |
| ◀ | lista de canais |
| ◀ ◀ (mais à esquerda) | lista de grupos |
| ▶ | Favoritos |
| ▶ ▶ (duas vezes rápido) | estatísticas do fluxo (ligar/desligar) |
| OK | painel de informação |
| OK outra vez | pausa |
| OK em pausa | continuar |
| OK longo | menu de ações (áudio, legendas, formato, definições) |
| números | ir para o canal pelo número |
| 0 | canal anterior |
| Voltar duas vezes | sair |

**Na lista de canais:**
- ▶ — guia do canal selecionado;
- OK longo — modo de marcação: ◀ adicionar/remover dos Favoritos, ▶ eliminar canal (os eliminados recuperam-se no grupo «Eliminados»).

**No smartphone:** toque — pausa e painel de informação; deslizar para cima — painel, para baixo — ocultá-lo; deslizar para a direita na metade esquerda — lista de canais; para a esquerda na metade direita — Favoritos; toque longo — definições.

---

## 4. Guia e arquivo

- O guia é guardado **24 horas para trás e 48 horas para a frente**.
- Prima ▶ na lista de canais para abrir o guia. Os programas passados podem ser vistos a partir do **arquivo**, se o fornecedor o suportar.
- No arquivo: **OK** — barra de avanço, ◀ ▶ — passo (acelera ao manter premido), **Voltar** — regressar ao direto.

---

## 5. Pausa do direto (Timeshift)

**Definições → Reprodução → Pausa ao vivo com gravação.**

- **Desligada:** a pausa congela a imagem; ao continuar, volta-se ao direto.
- **Ligada:** após a pausa, a reprodução continua **do mesmo momento**. O atraso em relação ao direto aparece em baixo; **Voltar** — regressar ao direto.

**Armazenamento da pausa:**
- **Memória interna** — a gravação começa no momento da pausa e é apagada ao mudar de canal.
- **Disco externo (USB)** — a gravação decorre sempre enquanto vê um canal, por isso **em pausa ◀ ▶ recuam** (até onde o espaço permitir). A aplicação cria a pasta `Timeshift` no disco e usa no máximo 80 % do espaço livre; as gravações antigas são apagadas automaticamente.

Pen USB: FAT32 ou exFAT (NTFS, se o dispositivo suportar).
Não são suportados fluxos DASH, fluxos encriptados e fluxos com faixa de áudio separada — nestes a pausa funciona normalmente.

---

## 6. Grupos ocultos (controlo parental)

1. Abra a lista de grupos (◀ ◀), escolha um grupo e **mantenha OK premido** — ativa-se a seleção de grupos.
2. Marque os grupos com OK e prima **Voltar**.
3. Introduza a palavra-passe com as setas e prima OK. A palavra-passe predefinida é **▶ ▶ ▶ ▶**.
4. Após a primeira ocultação, a aplicação propõe criar a sua própria palavra-passe de setas (ex. ▲ ▲ ◀ ▶) — memorize-a.

Para voltar a mostrar os grupos ocultos, na lista de grupos **prima ◀ três vezes rapidamente** e introduza a palavra-passe. Ao minimizar a aplicação, os grupos voltam a ficar ocultos.

---

## 7. Imagem na imagem e segundo plano (smartphone)

- **Imagem na imagem:** ao ir para o ecrã inicial, o vídeo continua numa janela pequena.
- **Áudio em segundo plano:** o áudio continua com o ecrã bloqueado; controlo na barra de notificações.

---

## 8. Definições

- **Ecrã:** taxa de fotogramas automática, 120 Hz, duração do painel de informação, deslocação das listas, **ecrã OLED** (proteção contra queima: deslocação de elementos, relógio oculto, proteção de ecrã em pausa, escurecimento dos menus).
- **Relógio:** posição no ecrã.
- **Reprodução:** imagem na imagem, áudio em segundo plano, nivelamento do volume, estatísticas, pausa do direto, pré-carregamento de canais vizinhos, buffer, User-Agent.
- **Temas** (botão «Temas» separado nas definições): temas prontos (Clássico, Preto OLED, Oceano, Quente, Vidro) ou cores próprias de painéis, seleção, texto, painel de informação, relógio e transparência.
- **Administração:** palavra-passe e bloqueio de opções (as opções bloqueadas ficam ocultas).

**User-Agent** é a forma como o leitor se «apresenta» ao servidor do fornecedor. Se a lista carrega mas os canais não abrem, experimente **VLC**.

---

## 9. Cópia de segurança

**Definições → Sobre → Exportar** guarda listas, Favoritos, grupos ocultos e definições num ficheiro. **Importar** restaura-os — por exemplo, num dispositivo novo.

---

## 10. Atualizações

- A aplicação verifica, descarrega e instala as atualizações sozinha (pode desligar em **Sobre**).
- A assinatura é verificada antes da instalação — uma atualização não pode ser falsificada.
- Se a aplicação não conseguir verificar atualizações durante **90 dias**, ativa-se um modo restrito (sem guia nem arquivo, 5 canais nos Favoritos). Basta ligar-se à internet — tudo volta.

---

## 11. Versão Pro

Neste momento todas as funções são **gratuitas**. Quando o Pro chegar, todos terão mais **3 meses** de acesso total.

| | Grátis | Pro |
|---|---|---|
| Qualidade | até 1080p (4K/HDR — 3 minutos) | 4K, HDR |
| Favoritos | 20 canais | sem limite |
| Grupos ocultos | 1 | sem limite |
| Arquivo | últimas 3 horas | o que o fornecedor oferecer |
| Nivelamento do volume, taxa automática, 120 Hz, AC3/DTS para o recetor | — | ✓ |
| Pausa ao vivo com gravação, temas | — | ✓ |
| Imagem na imagem e áudio em segundo plano (smartphone) | — | ✓ |

---

## 12. Resolução de problemas

- **Um canal não abre** — mude o User-Agent (VLC); teste a lista noutro dispositivo.
- **Sem guia** — verifique o endereço EPG na lista; abra **Listas** — o erro de carregamento aparece aí.
- **Áudio a crepitar no smartphone com nivelamento** — desligue o nivelamento.
- **4K aos solavancos numa TV box fraca** — escolha o buffer «Grande» ou veja em HD.

---

## 13. Ligar dispositivos e qualidade

- **Ligar dispositivos** (Definições → Ligar dispositivos): associe o telemóvel à TV com um código que aparece sozinho na TV. Envie listas e definições, adicione uma lista pelo navegador via QR, transmita do telemóvel para a TV (📺, o telemóvel vira comando) e traga a reprodução de volta.
- **Qualidade** (painel de informação): «Auto» baixa a qualidade com rede lenta; «Melhor» usa sempre a mais alta. Guardado por canal.
- **Buffer «Auto»**: cresce sozinho com paragens frequentes.

---

## 14. Conforto

- **Lembretes:** no guia, OK num programa futuro — marcado ◉, um minuto antes surge «Mudar».
- **Favoritos:** OK longo — ▲▼ reordenam, OK renomeia.
- **Programa no ecrã**, **tamanho da interface**, **arranque automático**, novo tema **«Néon»**.

---

© 2026 Ruslan G. Todos os direitos reservados.
