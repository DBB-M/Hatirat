---
title: Analizler
layout: page
permalink: /analizler.html
custom-foot: js/analizler-js.html
---

<h2 style="font-family:'EB Garamond',serif;color:#2a1f0e;margin-bottom:1.5rem;">Hatırat Envanteri: Analizler</h2>

<ul class="nav nav-tabs mb-4" id="analizTab" role="tablist">
  <li class="nav-item" role="presentation">
    <button class="nav-link active" data-bs-toggle="tab" data-bs-target="#frekans" type="button">Frekans</button>
  </li>
  <li class="nav-item" role="presentation">
    <button class="nav-link" data-bs-toggle="tab" data-bs-target="#zaman" type="button">Zaman</button>
  </li>
  <li class="nav-item" role="presentation">
    <button class="nav-link" data-bs-toggle="tab" data-bs-target="#ag" type="button">Ağlar</button>
  </li>
</ul>

<div class="tab-content">

  <div class="tab-pane fade show active" id="frekans">
    <div class="row g-4">
      <div class="col-md-6">
        <div class="card border-0 shadow-sm p-3">
          <h5 style="font-family:'EB Garamond',serif;color:#2a7f8c;">Türlere Göre Eser Sayısı</h5>
          <canvas id="chartTur"></canvas>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card border-0 shadow-sm p-3">
          <h5 style="font-family:'EB Garamond',serif;color:#2a7f8c;">En Sık Geçen Yazarlar (İlk 20)</h5>
          <canvas id="chartYazar"></canvas>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card border-0 shadow-sm p-3">
          <h5 style="font-family:'EB Garamond',serif;color:#2a7f8c;">En Sık Geçen Önemli Kişiler (İlk 20)</h5>
          <canvas id="chartKisi"></canvas>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card border-0 shadow-sm p-3">
          <h5 style="font-family:'EB Garamond',serif;color:#2a7f8c;">Başlıklarda En Sık Geçen Kelimeler</h5>
          <div id="kelimeCloud" style="line-height:2.4;padding:.5rem;min-height:200px;"></div>
        </div>
      </div>
    </div>
  </div>

  <div class="tab-pane fade" id="zaman">
    <div class="card border-0 shadow-sm p-3">
      <h5 style="font-family:'EB Garamond',serif;color:#2a7f8c;">Yıllara Göre Hatırat Üretimi (1854–2024)</h5>
      <canvas id="chartZaman"></canvas>
    </div>
  </div>

  <div class="tab-pane fade" id="ag">
    <div class="row g-4">
      <div class="col-12">
        <div class="card border-0 shadow-sm p-3">
          <h5 style="font-family:'EB Garamond',serif;color:#2a7f8c;">Yazar–Kişi Ağı</h5>
          <p class="text-muted small">Yazarlar ile eserlerinde adı geçen kişiler arasındaki ilişkiler</p>
          <div id="agYazarKisi" style="width:100%;height:500px;border:1px solid #e0d4b8;border-radius:8px;"></div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card border-0 shadow-sm p-3">
          <h5 style="font-family:'EB Garamond',serif;color:#2a7f8c;">Tür–Yazar Ağı</h5>
          <div id="agTurYazar" style="width:100%;height:450px;border:1px solid #e0d4b8;border-radius:8px;"></div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card border-0 shadow-sm p-3">
          <h5 style="font-family:'EB Garamond',serif;color:#2a7f8c;">Yayınevi–Tür Ağı</h5>
          <div id="agYayineviTur" style="width:100%;height:450px;border:1px solid #e0d4b8;border-radius:8px;"></div>
        </div>
      </div>
    </div>
  </div>

</div>
