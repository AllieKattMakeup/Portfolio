<!-- =====================================================================
     BANNER: drop your banner image into the images/ folder, then replace
     "images/YOUR_BANNER_HERE.jpg" below and remove the comment markers.
     ===================================================================== -->
<div style="width:100%;height:220px;background:linear-gradient(135deg,#f2cfe0,#d4a5bf);background-image:url('images/banner.jpg');background-size:cover;background-position:center;border-radius:10px;margin-bottom:2rem;"></div>

<div style="text-align:center;">

<img src="images/baddieallie.png" width="180" style="border-radius:50%;display:block;margin:0 auto 1rem;" alt="Allie — Makeup Artist">

# Makeup by Allie

*Soft glam · Editorial · Everyday looks · Special occasions*

Based in the Pacific Northwest &nbsp;|&nbsp; Available for bookings

[![Instagram](https://img.shields.io/badge/Instagram-@alliekatt.jpg.makeup-E1306C?style=flat&logo=instagram&logoColor=white)](https://www.instagram.com/alliekatt.jpg.makeup) <!---E1306C?style=flat&logo=instagram&logoColor=white-->

</div>

---

## About Me

Hi, I'm Allie 

I work with all skin tones and face shapes. Every look is customized to you.

---

## Services

| Service | Description |
|---|---|
| **Soft Glam** | Dewy skin, defined lashes, neutral-to-warm tones |
| **Editorial** | Bold, creative looks for shoots and events |
| **Everyday Glam** | Wearable, polished looks for day-to-day |
| **Special Occasion** | Weddings, quinceañeras, proms, events |

---

## Featured Look — Soft Glam

> Olive shimmer eye · Cat liner wing · Dewy skin · Neutral lip

<style>
.glam-carousel {
  max-width: 420px;
  margin: 2rem auto;
  text-align: center;
  font-family: inherit;
}
.glam-carousel img {
  width: 100%;
  max-width: 380px;
  border-radius: 8px;
  display: block;
  margin: 0.75rem auto;
}
.glam-label {
  font-size: 0.85rem;
  font-weight: 600;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  color: #888;
  margin-bottom: 0.25rem;
}
.glam-caption {
  font-size: 0.95rem;
  color: #555;
  margin: 0.4rem 0 0.75rem;
}
.glam-nav {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 1rem;
  margin-top: 0.5rem;
}
.glam-nav button {
  background: #1e1e1e;
  color: #fff;
  border: none;
  border-radius: 50%;
  width: 38px;
  height: 38px;
  font-size: 1.1rem;
  cursor: pointer;
  transition: background 0.2s;
}
.glam-nav button:hover { background: #555; }
.glam-counter {
  font-size: 0.85rem;
  color: #888;
  min-width: 3rem;
}
.glam-dots {
  display: flex;
  justify-content: center;
  gap: 6px;
  margin-top: 0.75rem;
}
.glam-dot {
  width: 8px;
  height: 8px;
  border-radius: 50%;
  background: #ccc;
  cursor: pointer;
  transition: background 0.2s;
}
.glam-dot.active { background: #1e1e1e; }
</style>

<div class="glam-carousel">
  <div id="glam-label" class="glam-label">Before</div>
  <img id="glam-img" src="images/frontbase.png" alt="Before — bare face">
  <div id="glam-caption" class="glam-caption">Bare skin, no makeup</div>
  <div class="glam-nav">
    <button onclick="glamMove(-1)">&#8592;</button>
    <span class="glam-counter"><span id="glam-cur">1</span> / 5</span>
    <button onclick="glamMove(1)">&#8594;</button>
  </div>
  <div class="glam-dots" id="glam-dots"></div>
</div>

<script>
(function() {
  var slides = [
    { src: "images/frontbase.png",  label: "Before",          caption: "Bare skin, no makeup" },
    { src: "images/frontopen.png",  label: "After",           caption: "Full look — eyes open" },
    { src: "images/frontupped.png", label: "After",           caption: "Eyeshadow detail — eyes closed" },
    { src: "images/betteriso.png",  label: "After",           caption: "Three-quarter angle" },
    { src: "images/isoangle.png",   label: "After",           caption: "Side angle" }
  ];
  var cur = 0;
  var img    = document.getElementById("glam-img");
  var label  = document.getElementById("glam-label");
  var cap    = document.getElementById("glam-caption");
  var curEl  = document.getElementById("glam-cur");
  var dotBox = document.getElementById("glam-dots");

  slides.forEach(function(_, i) {
    var d = document.createElement("span");
    d.className = "glam-dot" + (i === 0 ? " active" : "");
    d.onclick = function() { glamGoTo(i); };
    dotBox.appendChild(d);
  });

  function glamGoTo(n) {
    cur = (n + slides.length) % slides.length;
    img.src      = slides[cur].src;
    img.alt      = slides[cur].caption;
    label.textContent = slides[cur].label;
    cap.textContent   = slides[cur].caption;
    curEl.textContent = cur + 1;
    var dots = dotBox.querySelectorAll(".glam-dot");
    dots.forEach(function(d, i) {
      d.className = "glam-dot" + (i === cur ? " active" : "");
    });
  }

  window.glamMove = function(dir) { glamGoTo(cur + dir); };
})();
</script>

---

## More Work

<div style="text-align:center;">
<img src="images/single.png" width="380" style="border-radius:8px;" alt="Look — bold and confident">
</div>

---

## Book a Session

Interested in working together? Reach out via Instagram DM or email to check availability and pricing.

- **Instagram:** [@alliekatt.jpg.makeup](https://www.instagram.com/alliekatt.jpg.makeup?utm_source=ig_web_button_share_sheet&igsh=ZDNlZDc0MzIxNw==)
- **Email:** alliekattmakeup@gmail.com

> *All looks are done with professional-grade products. Skin prep and aftercare tips included with every session.*


