<template>
  <div class="contact-page">
    <div class="contact-card">
      <!-- Left: Info -->
      <div class="contact-info">
        <h3 class="info-title">Get In Touch</h3>

        <div class="info-item">
          <i class="fas fa-map-marker-alt"></i>
          <div>
            <span class="label">Address</span>
            <span class="value">Valhalla Park<br />Cape Town, CPT</span>
          </div>
        </div>

        <div class="info-item">
          <i class="fas fa-phone-alt"></i>
          <div>
            <span class="label">Let's Talk</span>
            <span class="value">068 196 6648</span>
          </div>
        </div>

        <div class="info-item">
          <i class="far fa-envelope"></i>
          <div>
            <span class="label">Queries</span>
            <span class="value">ashtonabrahams563@gmail.com</span>
          </div>
        </div>
      </div>

      <!-- Divider -->
      <div class="divider"></div>

      <!-- Right: Form -->
      <div class="contact-form">
        <h2>Contact Me</h2>

        <form action="https://formspree.io/f/mzboygza" method="POST">
          <div class="field">
            <label>Name *</label>
            <input type="text" name="Name" required placeholder="Your Name" />
          </div>

          <div class="field">
            <label>Email *</label>
            <input
              type="email"
              name="Email"
              required
              placeholder="Your Email"
            />
          </div>

          <div class="field">
            <label>Phone</label>
            <input type="tel" name="Phone" placeholder="Your Phone" />
          </div>

          <div class="field">
            <label>Subject *</label>
            <input type="text" name="Subject" required placeholder="Subject" />
          </div>

          <div class="field">
            <label>Message *</label>
            <textarea
              name="Message"
              rows="5"
              placeholder="Your Message"
            ></textarea>
          </div>

          <button type="submit">Send Message</button>
        </form>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.contact-page {
  padding-top: 110px;
  padding-bottom: 80px;
  display: flex;
  justify-content: center;
  color: #e5e7eb;
}

/* Main Card */
.contact-card {
  max-width: 1400px;
  width: 100%;
  margin: 0 32px;
  display: grid;
  grid-template-columns: 1fr auto 1.4fr;
  gap: 2.5rem;

  background: rgba(5, 6, 10, 0.6);
  border-radius: 22px;
  border: 1px solid rgba(255, 255, 255, 0.08);
  backdrop-filter: blur(14px);
  padding: 60px;
  box-shadow: 0 14px 34px rgba(0, 0, 0, 0.5);
}

/* Left Info */
.contact-info {
  display: flex;
  flex-direction: column;
  background-image: url(../images/Parallax.jpg);
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center;
  border-radius: 5px;
  gap: 28px;
  padding-left: 20px;
  padding-top: 10px;
}

.info-title {
  font-family: Space Grotesk, sans-serif;
  font-size: 1.8rem;
  color: #ffffff;
  text-decoration: underline;
  text-decoration-color: #7dd3fc;
  margin-bottom: 10px;
}

.info-item {
  display: flex;
  gap: 18px;
  align-items: flex-start;
  text-shadow:
    0 0 6px rgba(125, 211, 252, 0.8),
    0 0 10px rgba(167, 139, 250, 0.8);
}


.info-item i {
  font-size: 1.4rem;
  color: #7dd3fc;
  margin-top: 4px;
}

.label {
  font-family: Inter, sans-serif;
  font-size: 0.75rem;
  letter-spacing: 0.35em;
  text-transform: uppercase;
  color: #94a3b8;
}

.value {
  display: block;
  margin-top: 6px;
  font-size: 1rem;
  color: #cbd5f5;
}

/* Divider */
.divider {
  width: 1px;
  background: linear-gradient(
    to bottom,
    transparent,
    rgba(125, 211, 252, 0.5),
    transparent
  );
}

/* Form */
.contact-form h2 {
  font-family: Space Grotesk, sans-serif;
  font-size: 2.1rem;
  margin-bottom: 26px;
  text-decoration: underline;
  text-decoration-color: #7dd3fc;
}

.field {
  margin-bottom: 22px;
}

.contact-form label {
  display: block;
  margin-bottom: 8px;
  font-size: 0.75rem;
  letter-spacing: 0.25em;
  text-transform: uppercase;
  color: #94a3b8;
}

.contact-form input,
.contact-form textarea {
  width: 100%;
  padding: 10px 14px;
  border-radius: 10px;
  background: rgba(15, 23, 42, 0.65);
  border: 1px solid rgba(125, 211, 252, 0.35);
  color: #e5e7eb;
  font-size: 0.95rem;
}

.contact-form input:focus,
.contact-form textarea:focus {
  outline: none;
  border-color: #7dd3fc;
  box-shadow: 0 0 12px rgba(125, 211, 252, 0.35);
}

/* Button */
.contact-form button {
  margin-top: 12px;
  width: 100%;
  padding: 12px;
  border-radius: 999px;
  background: linear-gradient(90deg, #7dd3fc, #a78bfa);
  color: #020617;
  border: none;
  font-family: Inter, sans-serif;
  font-size: 0.75rem;
  letter-spacing: 0.35em;
  text-transform: uppercase;
  cursor: pointer;
  transition: transform 0.25s ease, box-shadow 0.25s ease;
}

.contact-form button:hover {
  transform: translateY(-2px);
  box-shadow: 0 0 18px rgba(125, 211, 252, 0.55);
}

/* Responsive */
@media (max-width: 900px) {
  .contact-card {
    grid-template-columns: 1fr;
    padding: 40px;
  }

  .divider {
    display: none;
  }
}
</style>
