---
title: CMN-GOMS
sections:
   - Modelo GOMS
---

No CMN-GOMS, há uma hierarquia estrita de objetivos, os operadores são
executados estritamente em ordem sequencial, e os métodos são representados numa
notação semelhante a um pseudocódigo, que inclui submétodos e condicionais.

Os objetivos e métodos foram numerados para facilitar sua identificação. Algarismos
indicam sequência, e letras indicam alternativas.

### Modelo GOMS

<div class="jumbotron">
<pre>
GOAL 0: descobrir informações sobre a cidade de Araguaina
	GOAL 1: encontrar secção sobre turismo
		METHOD 1.A: clicar na aba 'Araguaina' na barra de navegação
		(SEL. RULE: barra de navegação esta visivel)
		METHOD 1.B: clicar no botão 'TURISTA' na *sidebar*
		(SEL. RULE: usuario não encontra o link na *navbar* e *sidebar* esta visivel)
		METHOD 1.C: clicar no botão 'TURISTA' no *footer*
		(SEL. RULE: usuario não encontra o link na *navbar* e/ou *sidebar* e footer esta visivel)
	GOAL 2: obter informações sobre a cidade
		OP.2.1: examinar texto sobre historia da cidade
		OP.2.2: examinar texto sobre economia
		OP.2.3: examinar texto sobre emancipação
		OP.2.4: examinar texto sobre crescimento
		OP.2.5: examinar dados sobre o município de Araguaína
</pre>
</div>

Uma diferença importante entre os modelos KLM e CMN-GOMS é que o CMN-GOMS
é representado na forma de programa, e, portanto, a análise é geral e executável.
