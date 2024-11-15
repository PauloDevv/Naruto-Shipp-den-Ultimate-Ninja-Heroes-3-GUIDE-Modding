# Naruto Shippūden: Ultimate Ninja Heroes 3 GUIDE Modding

Este repositório contém informações detalhadas sobre a estrutura dos arquivos e pastas presentes na ISO do jogo **Naruto Shippūden: Ultimate Ninja Heroes 3**. O objetivo é servir como um guia para modding, facilitando a modificação e personalização do jogo.

---

## Estrutura Geral da ISO

A ISO é composta por:

- **PSP_GAME/** - Contém todos os arquivos importantes do jogo.
- **UMD_DATA.BIN** - Não possui relevância para modding por enquanto.

---

## Conteúdo da Pasta `PSP_GAME`

### Arquivos no Diretório Raiz

- **ICON0.PNG**  
  Ícone representativo do jogo *Naruto Shippūden: Ultimate Ninja Heroes 3*.

- **ICON1.PMF**  
  Arquivo de vídeo no formato PSMF (PlayStation Movie Format). Ele pode conter vídeos, cutscenes ou outros conteúdos.

- **PARAM.SFO**  
  Arquivo SFO (System File Object) utilizado pelo XMB para exibir informações e funcionalidades específicas ao executar o conteúdo.

- **PIC1.PNG**  
  Imagem ilustrativa do jogo.

- **SND0.AT3**  
  Pequeno arquivo de áudio, sem relevância para modding.

---

### Estrutura da Pasta `SYSDIR/`

- **EBOOT.BIN**  
  Arquivo ELF comprimido (executável principal do jogo).

- **BOOT.BIN**  
  Não possui relevância para modding.

- **OPNSSMP.BIN**  
  Função desconhecida, sem relevância para modding.

#### Arquivos Dentro da `SYSDIR/`:

- **EBOOT.BIN**  
  ELF comprimido para atualizações do jogo.

- **DATA.BIN**  
  Função desconhecida, sem relevância para modding.

---

### Estrutura da Pasta `USRDIR/`

A pasta **USRDIR** contém três subpastas e dois arquivos principais:

1. **Modules/**  
   - **libfont.prx**  
     Biblioteca de fontes.
   - **libsuppreacc.prx**  
     Função desconhecida, sem relevância para modding.

2. **Movie/**  
   - **logo_cc2.pmf**  
     Vídeo de introdução da CyberConnect2.
   - **logo_cri.pmf**  
     Logo da Criware.
   - **logo_nrt.pmf**  
     Conteúdo não utilizado.  
   - **MOVIE_01E.PMF** e similares:  
     Contêm as cutscenes do jogo.

3. **Sound/**  
   Não possui relevância, já que os arquivos de áudio estão nos arquivos **data.cpk** e **data.dns**.

- **data.cpk**  
  Contém arquivos dos personagens, menus e outros elementos principais.

- **data.dns**  
  Semelhante ao **data.cpk**, mas utilizado em atualizações no PSP.

---

## Descompactando o Arquivo `data.cpk`

Para descompactar o arquivo `data.cpk`, você precisará da ferramenta [YACpkTool](https://github.com/Brolijah/YACpkTool). Siga os passos abaixo:

1. Baixe a ferramenta no repositório do YACpkTool, seção **Releases**.
2. Extraia o arquivo `yacpktool.exe` e o coloque na mesma pasta do arquivo `data.cpk`.
3. Segure e arraste o arquivo `data.cpk` para o `yacpktool.exe`.  
   Isso irá descompactar o arquivo e gerar as pastas.

---

## Estrutura das Pastas Dentro do `data.cpk`

As pastas extraídas do **data.cpk** são:

- **00icon**  
- **01text**  
- **02boot**  
- **03font**  
- **04cmn**  
- **10loading**  
- **11mode**  
- **13adv**  
- **21btlsel**  
- **22vschr**  
- **30btlcmn**  
- **31btlstg**  
- **32btlchr**  
- **40skill**  
- **41spl**  
- **50btlend**  
- **sound**  

### Observação:
Ainda vou documentar o conteúdo dessas pastas em mais detalhes.

---

Contribuições para este guia são bem-vindas! Se você tem conhecimento sobre os arquivos do jogo ou deseja expandir as informações contidas aqui, sinta-se à vontade para abrir um pull request. 😊
