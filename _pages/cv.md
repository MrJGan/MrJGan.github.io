---
layout: portfolio-cv
permalink: /cv/
---
<div class="site-shell cv-page">
  <header class="site-header">
    <a class="wordmark" href="{{ '/' | relative_url }}" aria-label="Jing Gan home">JING GAN<span class="mark-dot">.</span></a>
    <nav aria-label="Main navigation">
      <a href="{{ '/' | relative_url }}">Home</a>
      <a href="{{ '/teaching/' | relative_url }}">Teaching</a>
    </nav>
  </header>

  <main id="main-content">
    <section class="cv-hero" aria-labelledby="cv-page-title">
      <p class="eyebrow"><span class="status-line"></span> PROFESSIONAL PROFILE <span class="eyebrow-slash">/</span> CV</p>
      <h1 id="cv-page-title">Curriculum <em>vitae</em></h1>
      <p class="cv-description">Research, academic training, professional experience, and teaching.</p>
    </section>

    <section class="cv-document" aria-label="Curriculum vitae PDF">
      <div class="cv-document-top">
        <div class="cv-document-heading">
          <span class="section-index">01 / DOCUMENT</span>
          <div class="cv-document-title">Jing Gan <span>· 3-page PDF</span></div>
        </div>
        <div class="cv-actions">
          <a class="cv-open" href="{{ '/files/Jing_Gan_CV.pdf' | relative_url }}" target="_blank" rel="noopener">OPEN PDF <span aria-hidden="true">↗</span></a>
          <a class="cv-download" href="{{ '/files/Jing_Gan_CV.pdf' | relative_url }}" download="Jing_Gan_CV.pdf">DOWNLOAD CV <span aria-hidden="true">↓</span></a>
        </div>
      </div>
      <div class="cv-preview">
        <iframe
          src="{{ '/files/Jing_Gan_CV.pdf' | relative_url }}#toolbar=1&navpanes=0&view=FitH"
          title="Preview of Jing Gan's curriculum vitae"
          loading="eager"
          width="100%"
          height="900"
          style="border: 0; display: block;"
        ></iframe>
      </div>
      <p class="cv-preview-help">If the preview is blank, please <a href="{{ '/files/Jing_Gan_CV.pdf' | relative_url }}" target="_blank" rel="noopener">open the PDF in a new tab ↗</a>. Your browser may be configured to download PDFs instead of displaying them.</p>
      <p class="cv-mobile-note">For easier reading on a phone, <a href="{{ '/files/Jing_Gan_CV.pdf' | relative_url }}" target="_blank" rel="noopener">open the PDF in a separate tab ↗</a></p>
    </section>
  </main>

  <footer class="site-footer">
    <span>© {{ 'now' | date: '%Y' }} JING GAN</span>
    <div><a href="mailto:jinggan@umass.edu">Email ↗</a><a href="{{ '/' | relative_url }}">Home ↗</a></div>
  </footer>
</div>
