/* =====================================================
   Maven Asset Management Solutions – Brand Styling
   ===================================================== */

/* Brand colors */
:root {
  --maven-blue-primary: #3e67b1;
  --maven-blue-deep: #292c75;
  --maven-gray-text: #545454;

  --background: #f6f8fb;
  --white: #ffffff;
  --border: #d9deea;
}

/* Reset */
* {
  box-sizing: border-box;
}

body {
  margin: 0;
  font-family: system-ui, -apple-system, Segoe UI, Roboto, Arial, sans-serif;
  color: var(--maven-gray-text);
  background: var(--background);
  line-height: 1.6;
}

/* Layout container */
.container {
  width: min(1100px, 92vw);
  margin: 0 auto;
}

/* =====================================================
   Header / Navigation
   ===================================================== */

.site-header {
  background: linear-gradient(
    90deg,
    var(--maven-blue-deep),
    var(--maven-blue-primary)
  );
  border-bottom: 1px solid rgba(255, 255, 255, 0.18);
}

.header-inner {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 14px 0;
  gap: 16px;
}

/* Logo */
.brand {
  display: flex;
  align-items: center;
  text-decoration: none;
}

.brand-logo {
  height: 40px;
  width: auto;
  display: block;
}

/* Navigation */
.nav {
  display: flex;
  gap: 18px;
  align-items: center;
  flex-wrap: wrap;
}

.nav a {
  color: #ffffff;
  font-weight: 600;
  font-size: 14px;
  text-decoration: none;
  padding: 6px 12px;
  border-radius: 999px;
  transition: background 0.2s ease, opacity 0.2s ease;
  opacity: 0.95;
}

.nav a:hover {
  background: rgba(255, 255, 255, 0.15);
  opacity: 1;
}

/* Active pill highlight */
.nav a.active {
  background: rgba(255, 255, 255, 0.22);
  border: 1px solid rgba(255, 255, 255, 0.35);
}

/* CTA button */
.nav .cta {
  background: rgba(255, 255, 255, 0.18);
  border: 1px solid rgba(255, 255, 255, 0.25);
  font-weight: 700;
}

.nav .cta:hover {
  background: rgba(255, 255, 255, 0.28);
}

/* =====================================================
   Main Content
   ===================================================== */

main.container {
  padding: 28px 0 46px;
}

/* Hero */
.hero {
  background: var(--maven-blue-deep);
  color: #ffffff;
  border-radius: 14px;
  padding: 34px;
}

.hero h1 {
  margin: 0 0 10px;
  font-size: 36px;
}

.hero p {
  margin: 0;
  max-width: 760px;
  color: rgba(255, 255, 255, 0.92);
}

/* =====================================================
   Cards / Grid
   ===================================================== */

.grid {
  display: grid;
  grid-template-columns: 1.2fr 1fr 1fr;
  gap: 18px;
  margin-top: 18px;
}

.card {
  background: var(--white);
  border: 1px solid var(--border);
  border-radius: 14px;
  padding: 18px;
  box-shadow: 0 6px 20px rgba(41, 44, 117, 0.08);
}

.card h2 {
  margin: 0 0 10px;
  font-size: 18px;
  color: var(--maven-blue-deep);
}

.card p {
  margin: 0 0 12px;
}

.card ul {
  margin: 0;
  padding-left: 18px;
}

.card li {
  margin: 8px 0;
}

/* Buttons */
.button {
  display: inline-block;
  background: var(--maven-blue-primary);
  color: #ffffff;
  font-weight: 700;
  padding: 10px 16px;
  border-radius: 10px;
  text-decoration: none;
  transition: background 0.2s ease;
}

.button:hover {
  background: var(--maven-blue-deep);
}

/* Section label */
.section-title {
  margin: 22px 0 10px;
  font-size: 13px;
  color: var(--maven-gray-text);
  text-transform: uppercase;
  letter-spacing: 0.08em;
}

/* =====================================================
   SQL Reference Block
   ===================================================== */

.maven-sql {
  position: relative;
  background: #f4f6fb;
  border: 1px solid var(--border);
  border-left: 5px solid var(--maven-blue-primary);
  border-radius: 12px;
  padding: 20px;
  margin: 24px 0;
  overflow-x: auto;
  font-family: Consolas, Monaco, monospace;
  font-size: 13.5px;
  line-height: 1.5;
}

.maven-sql-header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 12px;
}

.maven-sql-label {
  font-size: 11px;
  font-weight: 800;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  color: var(--maven-blue-deep);
}

.maven-sql-meta {
  font-size: 11px;
  font-weight: 600;
  color: var(--maven-gray-text);
}

.maven-sql code {
  display: block;
  white-space: pre;
  color: #1a1a1a;
}

.maven-copy-btn {
  background: var(--maven-blue-primary);
  color: #ffffff;
  border: none;
  padding: 6px 14px;
  border-radius: 999px;
  font-size: 12px;
  font-weight: 700;
  cursor: pointer;
  transition: background 0.2s ease;
}

.maven-copy-btn:hover {
  background: var(--maven-blue-deep);
}

/* =====================================================
   Footer
   ===================================================== */

.site-footer {
  background: #ffffff;
  border-top: 1px solid var(--border);
  padding: 24px 0;
}

.footer-inner {
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap: 18px;
  flex-wrap: wrap;
}

.footer-left {
  flex: 1;
  min-width: 250px;
}

.footer-right {
  display: flex;
  align-items: center;
  gap: 14px;
  flex-wrap: wrap;
  justify-content: flex-end;
}

/* Follow label */
.footer-follow {
  display: flex;
  flex-direction: column;
  align-items: flex-end;
  gap: 6px;
}

.footer-follow-label {
  font-size: 11px;
  font-weight: 800;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  color: var(--maven-gray-text);
  opacity: 0.85;
}

/* Social icons */
.footer-social {
  display: flex;
  gap: 10px;
}

.social-link {
  width: 34px;
  height: 34px;
  border-radius: 999px;
  display: inline-flex;
  align-items: center;
  justify-content: center;
  background: rgba(62, 103, 177, 0.12);
  border: 1px solid rgba(217, 222, 234, 0.9);
  transition: transform 0.15s ease, background 0.15s ease;
}

.social-link svg {
  width: 16px;
  height: 16px;
  fill: var(--maven-blue-deep);
}

.social-link:hover {
  transform: translateY(-2px);
  background: rgba(62, 103, 177, 0.18);
}

/* =====================================================
   Responsive
   ===================================================== */

@media (max-width: 900px) {
  .grid {
    grid-template-columns: 1fr;
  }

  .hero h1 {
    font-size: 28px;
  }

  .nav {
    gap: 12px;
  }

  .footer-inner {
    flex-direction: column;
    align-items: flex-start;
  }

  .footer-follow {
    align-items: flex-start;
  }
}
