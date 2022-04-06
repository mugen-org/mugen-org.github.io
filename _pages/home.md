---
layout: default
permalink: "/"
---

<link rel="stylesheet" type="text/css" href="/static/css/home.css">

<div class="container">
  <div class="row">
    <!-- Teaser figure -->
    <div class="col-md-6 col-sm-6 col-xs-6 col-12">
      <!-- <img alt="{{ site.title }}" title="{{ site.title }}" id="teaser-figure" src="/static/img/paper/teaser.jpg"> -->
      <video width="512" height="512" controls>
      <source src="static/video/MUGEN_final.mp4" type="video/mp4">
      </video>
      <p id="teaser-caption">
        An overview of MUGEN.
      </p>
    </div>
    <!-- Abstract -->
    <div class="col-md-6 col-sm-6 col-xs-6 col-12">
      <p>
      Multimodal video-audio-text understanding and generation can benefit from datasets that are narrow but rich. The narrowness allows bite-sized challenges that the research community can make progress on. The richness ensures we are making progress along the core challenges. To this end, we present a large-scale video-audio-text dataset MUGEN, collected using the open-sourced platform game <a href="https://github.com/openai/coinrun">CoinRun</a>. We made substantial modifications to make the game richer by introducing audio and enabling new interactions. We trained RL agents with different objectives to navigate the game and interact with 13 objects and characters. This allows us to automatically extract a large collection of diverse videos and associated audio. We sample 375K video clips (3.2s each) and collect text descriptions from human annotators. Each video has additional annotations that are extracted automatically from the game engine, such as accurate semantic maps for each frame and templated textual descriptions Altogether, MUGEN can help progress research in many tasks in multimodal understanding and generation. We benchmark representative approaches on tasks involving video-audio-text retrieval and generation. Both MUGEN and the enhanced game engine will be released to serve as a playground for multimodal research.
      </p>
    </div>
  </div>
</div>

<hr>

<h2 class="anchor" id="people">Team</h2>
<div class="people-container">
{% include people.html %}
</div>
<hr>

<h2 class="anchor" id="citation">Citation</h2>
  <div class="paper-title col-md-12 col-sm-12 col-xs-12">
    MUGEN: A Playground for Video-Audio-Text Multimodal Understanding and GENeration
  </div>
  <!-- negative margin to account for superscripted asterisk -->
  <div class="paper-authors col-md-12 col-sm-12 col-xs-12" style="margin-top: -4px;">
    Thomas Hayes<sup>*</sup>, Songyang Zhang<sup>*</sup>, Xi Yin, Guan Pang, Sasha Sheng, Harry Yang, Songwei Ge, Isabelle Hu, Devi Parikh
  </div>
  <!-- arxiv and website link -->
  <div class="paper-links col-md-12 col-sm-12 col-xs-12">
    <span class="paper-link">
      <b>Arxiv</b>
    </span>
    <a class="paper-link button-div" href="/static/bibliography/nocaps_bibtex.txt" target="_blank">
      bibtex
    </a>
    <a class="paper-link button-div" href="/static/bibliography/nocaps_natbib.txt" target="_blank">
      natbib
    </a>
  </div>

<hr>

<br/>