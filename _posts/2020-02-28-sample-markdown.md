---
layout: post
title: Sample blog post to learn markdown tips
subtitle: There's lots to learn!
gh-repo: daattali/beautiful-jekyll
gh-badge: [star, fork, follow]
tags: [test]
comments: true
mathjax: true
author: Bill Smith
---

{: .box-success}
Era uma vez, em uma cidade pequena e tranquila, onde as ruas eram pavimentadas com pedras irregulares e as casas eram de cores vibrantes, um objeto curioso e peculiar chamava a atenção de todos: o lendário paralelepipado. Este não era um paralelepípedo comum, como aqueles que se encontram em calçadas e praças. O paralelepipado tinha uma aura mágica, irradiando uma luz suave e multicolorida que parecia dançar nas superfícies ao redor.

Dizia-se que o paralelepipado havia sido descoberto por um explorador excêntrico, o Senhor Bartholomeu Quimérico, durante uma de suas expedições às profundezas de uma floresta misteriosa. Bartholomeu, conhecido por sua paixão por artefatos enigmáticos, ficara fascinado pelo objeto de imediato. Tinha certeza de que aquele paralelepipado era uma chave para um mundo de possibilidades infinitas.

Bartholomeu levou o paralelepipado de volta à sua cidade natal, onde começou a estudá-lo minuciosamente. Construiu um laboratório improvisado em sua casa, recheado de livros antigos, ferramentas esquisitas e diagramas complexos. Ele acreditava que o paralelepipado possuía poderes extraordinários que poderiam ser desbloqueados com o conhecimento certo.

Enquanto isso, os moradores da cidade começaram a contar histórias fantásticas sobre o paralelepipado. Uns diziam que ele podia conceder desejos, outros que era capaz de revelar segredos ocultos do universo. As crianças, por sua vez, adoravam inventar contos de aventuras onde o paralelepipado era a chave para reinos mágicos e tesouros escondidos.

Um dia, enquanto Bartholomeu trabalhava em uma fórmula alquímica, algo extraordinário aconteceu. O paralelepipado começou a brilhar com uma intensidade jamais vista antes. As cores se misturavam em um espetáculo hipnótico e, de repente, uma porta luminosa surgiu no ar. Bartholomeu, com o coração batendo forte, atravessou a porta e se encontrou em um mundo maravilhoso, cheio de criaturas fantásticas e paisagens deslumbrantes.

Naquele mundo, Bartholomeu descobriu que o paralelepipado era, na verdade, uma peça de um quebra-cabeça cósmico, e ele era o escolhido para resolver esse enigma. Durante sua jornada, encontrou aliados inusitados, enfrentou desafios incríveis e desvendou mistérios antigos. Cada passo que dava, aproximava-o mais da compreensão total do paralelepipado e de seus próprios limites.

Ao final de sua aventura, Bartholomeu retornou à sua cidade, trazendo consigo não apenas o conhecimento adquirido, mas também um novo paralelepipado, uma espécie de presente do outro mundo. Ele compartilhou suas descobertas com os moradores, que passaram a ver o mundo com novos olhos, inspirados pela magia e pelas possibilidades infinitas que o paralelepipado representava.

E assim, a pequena cidade, que antes era apenas um ponto tranquilo no mapa, tornou-se um centro de curiosidade e inspiração, tudo graças ao enigmático paralelepipado e ao espírito aventureiro do Senhor Bartholomeu Quimérico. [take 5 minutes to learn how to write in markdown](https://markdowntutorial.com/) - it'll teach you how to transform regular text into bold/italics/tables/etc.<br/>I also encourage you to look at the [code that created this post](https://raw.githubusercontent.com/daattali/beautiful-jekyll/master/_posts/2020-02-28-sample-markdown.md) to learn some more advanced tips about using markdown in Beautiful Jekyll.

**Here is some bold text**

## Here is a secondary heading

[This is a link to a different site](https://deanattali.com/) and [this is a link to a section inside this page](#local-urls).

Here's a table:

| Number | Next number | Previous number |
| :------ |:--- | :--- |
| Five | Six | Four |
| Ten | Eleven | Nine |
| Seven | Eight | Six |
| Two | Three | One |

You can use [MathJax](https://www.mathjax.org/) to write LaTeX expressions. For example:
When \\(a \ne 0\\), there are two solutions to \\(ax^2 + bx + c = 0\\) and they are $$x = {-b \pm \sqrt{b^2-4ac} \over 2a}.$$

How about a yummy crepe?

![Crepe](https://beautifuljekyll.com/assets/img/crepe.jpg)

It can also be centered!

![Crepe](https://beautifuljekyll.com/assets/img/crepe.jpg){: .mx-auto.d-block :}

Here's a code chunk:

~~~
var foo = function(x) {
  return(x + 5);
}
foo(3)
~~~

And here is the same code with syntax highlighting:

```javascript
var foo = function(x) {
  return(x + 5);
}
foo(3)
```

And here is the same code yet again but with line numbers:

{% highlight javascript linenos %}
var foo = function(x) {
  return(x + 5);
}
foo(3)
{% endhighlight %}

## Boxes
You can add notification, warning and error boxes like this:

### Notification

{: .box-note}
**Note:** This is a notification box.

### Warning

{: .box-warning}
**Warning:** This is a warning box.

### Error

{: .box-error}
**Error:** This is an error box.

## Local URLs in project sites {#local-urls}

When hosting a *project site* on GitHub Pages (for example, `https://USERNAME.github.io/MyProject`), URLs that begin with `/` and refer to local files may not work correctly due to how the root URL (`/`) is interpreted by GitHub Pages. You can read more about it [in the FAQ](https://beautifuljekyll.com/faq/#links-in-project-page). To demonstrate the issue, the following local image will be broken **if your site is a project site:**

![Crepe](/assets/img/crepe.jpg)

If the above image is broken, then you'll need to follow the instructions [in the FAQ](https://beautifuljekyll.com/faq/#links-in-project-page). Here is proof that it can be fixed:

![Crepe]({{ '/assets/img/crepe.jpg' | relative_url }})
