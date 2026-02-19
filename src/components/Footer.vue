<template>
  <footer class="footer">
    <div class="footer-inner">
      <div class="footer-left">
        <p class="copyright">© 2026 Ashton Abrahams — All rights reserved</p>
      </div>

      <div class="footer-right">
        <nav class="footer-nav" aria-label="Footer navigation">
          <router-link class="footer-link" to="/">Home</router-link>
          <router-link class="footer-link" to="/contact">Contact</router-link>
        </nav>

        <div class="footer-connect">
          <span class="follow">Follow me</span>

          <a
            href="https://www.facebook.com/profile.php?id=100085302518838"
            target="_blank"
            class="social-icon"
            aria-label="Facebook"
          >
            <i class="fab fa-facebook-f"></i>
          </a>

          <a
            href="https://twitter.com/ASHTON_M_DB9"
            target="_blank"
            class="social-icon"
            aria-label="Twitter/X"
          >
            <i class="fab fa-twitter"></i>
          </a>

          <a
            href="https://www.instagram.com/ashton.m_db9/"
            target="_blank"
            rel="noopener noreferrer"
            class="social-icon"
            aria-label="Instagram"
          >
            <i class="fab fa-instagram"></i>
          </a>

          <a
            href="https://github.com/ASHTONMDB9"
            target="_blank"
            rel="noopener noreferrer"
            class="social-icon"
            aria-label="GitHub"
          >
            <i class="fab fa-github"></i>
          </a>

          <a
            href="https://www.linkedin.com/in/ashton-abrahams-0bb921237/"
            target="_blank"
            rel="noopener noreferrer"
            class="social-icon"
            aria-label="Linked In"
          >
            <i class="fab fa-linkedin"></i>
          </a>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {};
</script>

<style>
.footer {
  position: fixed;
  bottom: 0;
  width: 100%;
  z-index: 10;
  padding: 12px 24px;
  background: rgba(5, 6, 10, 0.6);
  backdrop-filter: blur(10px);
  border-top: 1px solid rgba(255, 255, 255, 0.06);
}

.footer-inner {
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap: 1rem;
  max-width: 1500px;
  margin: 0 auto;
}

.footer-left {
  flex: 1;
}

.footer-right {
  display: flex;
  align-items: center;
  gap: 1.4rem;
}

.footer-nav {
  display: flex;
  gap: 1.2rem;
  align-items: center;
}

.copyright {
  color: #94a3b8;
}

.footer-link {
  font-family: Inter, sans-serif;
  font-size: 0.75rem;
  letter-spacing: 0.35em;
  text-transform: uppercase;
  color: #cbd5f5;
  transition: color 0.3s ease;
}

.footer-link:hover {
  color: #7dd3fc;
}

.follow {
  font-family: Inter, sans-serif;
  font-size: 0.75rem;
  letter-spacing: 0.25em;
  color: #94a3b8;
  text-transform: uppercase;
}

.footer-connect {
  display: flex;
  gap: 0.7rem;
  align-items: center;
}

.social-icon {
  width: 36px;
  height: 36px;
  display: grid;
  place-items: center;
  border-radius: 50%;
  border: 1px solid rgba(125, 211, 252, 0.35);
  color: #cbd5f5;
  text-decoration: none;
  transition: transform 0.25s ease, box-shadow 0.25s ease,
    border-color 0.25s ease;
}

.social-icon:hover {
  color: #e0f2fe;
  transform: scale(1.1);
  box-shadow: 0 0 14px rgba(125, 211, 252, 0.35),
    0 0 26px rgba(167, 139, 250, 0.35);
  border-color: rgba(167, 139, 250, 0.8);
}

.social-icon i {
  font-size: 15px;
}
</style>
