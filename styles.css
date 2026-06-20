:root {
  --yellow: #ffbe22;
  --yellow-soft: #fff3c8;
  --yellow-pale: #fffaf0;
  --black: #17140f;
  --ink: #342e24;
  --muted: #756d61;
  --cream: #fffdf8;
  --white: #ffffff;
  --line: #ece5d8;
  --green: #2f7652;
  --green-soft: #e7f5ec;
  --orange: #d96b1d;
  --orange-soft: #fff0df;
  --red: #b9362d;
  --red-soft: #ffebe8;
  --shadow: 0 22px 60px rgba(74, 54, 16, 0.1);
}

* {
  box-sizing: border-box;
}

html {
  scroll-behavior: smooth;
}

body {
  min-width: 320px;
  min-height: 100vh;
  margin: 0;
  overflow-x: hidden;
  color: var(--black);
  background:
    linear-gradient(180deg, rgba(255, 190, 34, 0.08), transparent 26rem),
    var(--cream);
  font-family: "Arial Rounded MT Bold", "PingFang SC", "Microsoft YaHei", system-ui, sans-serif;
}

button,
input,
select {
  font: inherit;
}

button {
  cursor: pointer;
}

.sun-blob {
  position: fixed;
  z-index: -1;
  border-radius: 50%;
  filter: blur(2px);
  pointer-events: none;
}

.sun-blob-one {
  top: -230px;
  right: -180px;
  width: 540px;
  height: 540px;
  background: rgba(255, 190, 34, 0.17);
}

.sun-blob-two {
  bottom: -260px;
  left: -210px;
  width: 500px;
  height: 500px;
  background: rgba(255, 220, 119, 0.17);
}

.app {
  width: min(1120px, calc(100% - 40px));
  min-height: calc(100vh - 90px);
  margin: 0 auto;
}

.brand {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 18px;
  padding: 25px 0;
}

.brand-mark {
  display: inline-flex;
  align-items: center;
  gap: 8px;
  color: var(--black);
  font-size: 1.35rem;
  font-weight: 1000;
  letter-spacing: 0.03em;
  text-decoration: none;
}

.paw {
  position: relative;
  display: grid;
  width: 35px;
  height: 35px;
  place-items: center;
  border-radius: 50%;
  color: var(--black);
  background: var(--yellow);
  font-size: 0.65rem;
}

.paw::before {
  content: "•••";
  position: absolute;
  top: 1px;
  left: 7px;
  letter-spacing: 1px;
}

.brand-tag {
  color: var(--muted);
  font-size: 0.78rem;
  font-weight: 700;
}

.screen {
  display: none;
  animation: appear 240ms ease;
}

.screen.active {
  display: block;
}

@keyframes appear {
  from {
    opacity: 0;
    transform: translateY(8px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

.hero {
  display: grid;
  grid-template-columns: 1.05fr 0.95fr;
  align-items: center;
  gap: 50px;
  min-height: 570px;
  padding: 45px 0 65px;
}

.pill,
.risk-label {
  display: inline-flex;
  align-items: center;
  border-radius: 999px;
  font-size: 0.76rem;
  font-weight: 900;
  letter-spacing: 0.02em;
}

.pill {
  padding: 8px 13px;
  background: var(--yellow-soft);
}

h1,
h2,
h3,
p {
  margin-top: 0;
}

h1 {
  max-width: 670px;
  margin: 24px 0 22px;
  font-size: clamp(3rem, 7vw, 5.8rem);
  line-height: 0.98;
  letter-spacing: -0.07em;
}

.hero-copy > p {
  max-width: 570px;
  margin-bottom: 28px;
  color: var(--muted);
  font-size: 1.04rem;
  line-height: 1.8;
}

.primary-button,
.secondary-button,
.small-button,
.back-button {
  border: 0;
  transition: 160ms ease;
}

.primary-button {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  gap: 22px;
  min-height: 54px;
  padding: 0 24px;
  border-radius: 16px;
  color: var(--black);
  background: var(--yellow);
  box-shadow: 0 11px 24px rgba(255, 190, 34, 0.26);
  font-weight: 900;
}

.primary-button:hover,
.answer-option:hover {
  transform: translateY(-2px);
  box-shadow: 0 14px 28px rgba(255, 190, 34, 0.3);
}

.primary-button span {
  font-size: 1.2rem;
}

.privacy-note {
  margin: 16px 0 0 !important;
  font-size: 0.72rem !important;
}

.pet-visual {
  position: relative;
  min-height: 470px;
}

.yellow-disc {
  position: absolute;
  top: 34px;
  right: 6%;
  width: 390px;
  max-width: 88%;
  aspect-ratio: 1;
  border-radius: 50%;
  background:
    radial-gradient(circle at 36% 30%, #ffd65d, transparent 28%),
    var(--yellow);
}

.pet-card {
  position: absolute;
  display: flex;
  align-items: center;
  flex-direction: column;
  justify-content: center;
  width: 190px;
  height: 235px;
  border: 5px solid var(--white);
  border-radius: 100px 100px 34px 34px;
  background: rgba(255, 255, 255, 0.92);
  box-shadow: var(--shadow);
}

.pet-card strong {
  margin-top: 7px;
}

.pet-emoji {
  font-size: 6rem;
  filter: drop-shadow(0 8px 10px rgba(0, 0, 0, 0.08));
}

.dog-card {
  top: 56px;
  left: 5%;
  transform: rotate(-4deg);
}

.cat-card {
  right: 4%;
  bottom: 24px;
  transform: rotate(5deg);
}

.gut-badge {
  position: absolute;
  right: 38%;
  bottom: 60px;
  z-index: 2;
  display: flex;
  align-items: center;
  gap: 9px;
  padding: 13px 17px;
  border-radius: 15px;
  color: var(--white);
  background: var(--black);
  box-shadow: 0 12px 32px rgba(23, 20, 15, 0.22);
  transform: rotate(-3deg);
}

.gut-badge span {
  color: var(--yellow);
}

.home-benefits {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  border-top: 1px solid var(--line);
}

.home-benefits article {
  padding: 30px 28px;
  border-right: 1px solid var(--line);
}

.home-benefits article:last-child {
  border-right: 0;
}

.home-benefits span {
  display: block;
  margin-bottom: 12px;
  color: var(--yellow);
  font-weight: 1000;
}

.home-benefits strong {
  display: block;
  margin-bottom: 7px;
}

.home-benefits p {
  margin: 0;
  color: var(--muted);
  font-size: 0.79rem;
}

.step-head {
  display: grid;
  grid-template-columns: 42px 1fr 46px;
  align-items: center;
  gap: 15px;
  width: min(720px, 100%);
  margin: 25px auto 20px;
}

.back-button {
  width: 42px;
  height: 42px;
  border: 1px solid var(--line);
  border-radius: 50%;
  color: var(--black);
  background: var(--white);
  font-size: 1.15rem;
}

.progress-track {
  height: 8px;
  overflow: hidden;
  border-radius: 99px;
  background: #eee8dc;
}

.progress-track span {
  display: block;
  height: 100%;
  border-radius: inherit;
  background: var(--yellow);
  transition: width 220ms ease;
}

.step-count {
  color: var(--muted);
  font-size: 0.72rem;
  font-weight: 800;
  text-align: right;
}

.content-card,
.quiz-card {
  width: min(680px, 100%);
  margin: 0 auto 60px;
  padding: 42px;
  border: 1px solid rgba(236, 229, 216, 0.95);
  border-radius: 28px;
  background: rgba(255, 255, 255, 0.95);
  box-shadow: var(--shadow);
}

.eyebrow {
  margin-bottom: 9px;
  color: #bd8610;
  font-size: 0.72rem;
  font-weight: 1000;
  letter-spacing: 0.14em;
}

h2 {
  margin-bottom: 10px;
  font-size: clamp(1.85rem, 5vw, 2.75rem);
  line-height: 1.12;
  letter-spacing: -0.045em;
}

.section-intro,
.question-help,
.result-top p {
  color: var(--muted);
  line-height: 1.65;
}

fieldset {
  padding: 0;
  margin: 30px 0 22px;
  border: 0;
}

legend,
.field > span {
  display: block;
  margin-bottom: 9px;
  color: var(--ink);
  font-size: 0.8rem;
  font-weight: 850;
}

.pet-selector {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 12px;
}

.pet-selector input {
  position: absolute;
  opacity: 0;
}

.pet-selector label span {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 12px;
  min-height: 78px;
  border: 2px solid var(--line);
  border-radius: 17px;
  background: var(--white);
  font-weight: 900;
  transition: 160ms ease;
}

.pet-selector label b {
  font-size: 1.8rem;
}

.pet-selector input:checked + span {
  border-color: var(--yellow);
  background: var(--yellow-soft);
  box-shadow: 0 0 0 3px rgba(255, 190, 34, 0.15);
}

.field {
  display: block;
  margin-bottom: 18px;
}

.field-row {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 14px;
}

input,
select {
  width: 100%;
  height: 52px;
  padding: 0 15px;
  border: 1.5px solid var(--line);
  border-radius: 13px;
  outline: none;
  color: var(--black);
  background: #fffefb;
}

input:focus,
select:focus {
  border-color: var(--yellow);
  box-shadow: 0 0 0 4px rgba(255, 190, 34, 0.13);
}

.full-button {
  width: 100%;
  margin-top: 10px;
}

.quiz-card {
  min-height: 500px;
  text-align: center;
}

.question-icon {
  display: grid;
  width: 70px;
  height: 70px;
  margin: 0 auto 23px;
  place-items: center;
  border-radius: 22px;
  background: var(--yellow-soft);
  font-size: 2rem;
}

.question-help {
  min-height: 26px;
  margin-bottom: 26px;
  font-size: 0.87rem;
}

.answer-list {
  display: grid;
  gap: 10px;
  text-align: left;
}

.answer-option {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 14px;
  width: 100%;
  min-height: 58px;
  padding: 12px 17px;
  border: 1.5px solid var(--line);
  border-radius: 14px;
  color: var(--ink);
  background: var(--white);
  font-weight: 750;
  text-align: left;
  transition: 150ms ease;
}

.answer-option span {
  display: grid;
  flex: 0 0 27px;
  width: 27px;
  height: 27px;
  place-items: center;
  border-radius: 50%;
  color: var(--muted);
  background: #f6f1e8;
}

.answer-option.selected {
  border-color: var(--yellow);
  background: var(--yellow-soft);
}

.result-top {
  display: flex;
  align-items: flex-start;
  justify-content: space-between;
  gap: 20px;
  padding: 34px 0 24px;
}

.result-top h2 {
  margin-bottom: 7px;
}

.result-top p {
  margin: 0;
  font-size: 0.8rem;
}

.small-button,
.secondary-button {
  min-height: 43px;
  padding: 0 16px;
  border: 1px solid var(--line);
  border-radius: 12px;
  color: var(--black);
  background: var(--white);
  font-weight: 850;
}

.result-hero {
  display: grid;
  grid-template-columns: auto 1fr;
  align-items: center;
  gap: 30px;
  padding: 34px;
  border-radius: 27px;
  background: var(--yellow-soft);
}

.score-ring {
  display: grid;
  width: 130px;
  height: 130px;
  place-content: center;
  border: 10px solid rgba(255, 255, 255, 0.75);
  border-radius: 50%;
  background: var(--yellow);
  text-align: center;
}

.score-ring span {
  display: block;
  font-size: 2.7rem;
  font-weight: 1000;
  line-height: 0.95;
}

.score-ring small {
  color: #65521c;
  font-weight: 800;
}

.risk-label {
  margin-bottom: 10px;
  padding: 7px 11px;
  background: rgba(255, 255, 255, 0.7);
}

.result-hero h3 {
  margin-bottom: 7px;
  font-size: 1.55rem;
}

.result-hero p {
  max-width: 620px;
  margin: 0;
  color: var(--ink);
  line-height: 1.65;
}

.result-hero.low {
  background: var(--green-soft);
}

.result-hero.watch,
.result-hero.moderate {
  background: var(--orange-soft);
}

.result-hero.high {
  background: var(--red-soft);
}

.alert-box {
  margin-top: 16px;
  padding: 18px 20px;
  border: 1px solid #f3bbb5;
  border-radius: 16px;
  color: #79251f;
  background: var(--red-soft);
}

.alert-box p {
  margin: 7px 0 0;
  line-height: 1.6;
}

.report-grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 16px;
  margin-top: 16px;
}

.report-card {
  padding: 26px;
  border: 1px solid var(--line);
  border-radius: 20px;
  background: var(--white);
}

.advice-card {
  grid-column: 1 / -1;
  background: var(--yellow-pale);
}

.card-title {
  display: flex;
  align-items: center;
  gap: 10px;
  margin-bottom: 18px;
}

.card-title span {
  font-size: 1.2rem;
}

.card-title h3 {
  margin: 0;
  font-size: 1rem;
}

dl {
  margin: 0;
}

dl div {
  display: flex;
  justify-content: space-between;
  gap: 18px;
  padding: 10px 0;
  border-bottom: 1px solid #f1ece4;
  font-size: 0.82rem;
}

dl div:last-child {
  border-bottom: 0;
}

dt {
  color: var(--muted);
}

dd {
  margin: 0;
  font-weight: 800;
  text-align: right;
}

.finding-list,
.report-card ul {
  padding: 0;
  margin: 0;
  list-style: none;
}

.finding-list li,
.report-card ul li {
  position: relative;
  padding: 9px 0 9px 25px;
  color: var(--ink);
  font-size: 0.86rem;
  line-height: 1.55;
}

.finding-list li::before,
.report-card ul li::before {
  content: "✓";
  position: absolute;
  top: 9px;
  left: 0;
  color: #bb8205;
  font-weight: 1000;
}

.result-actions {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 12px;
  margin: 20px 0;
}

.medical-note {
  padding: 20px;
  border-radius: 16px;
  color: var(--muted);
  background: #f5f2ec;
  font-size: 0.76rem;
  line-height: 1.6;
}

.medical-note p {
  margin: 7px 0 0;
}

footer {
  display: flex;
  justify-content: space-between;
  gap: 20px;
  width: min(1120px, calc(100% - 40px));
  margin: 0 auto;
  padding: 30px 0;
  color: var(--muted);
  font-size: 0.68rem;
}

.toast {
  position: fixed;
  right: 20px;
  bottom: 20px;
  z-index: 5;
  padding: 12px 16px;
  border-radius: 12px;
  color: white;
  background: var(--black);
  box-shadow: var(--shadow);
  opacity: 0;
  pointer-events: none;
  transform: translateY(10px);
  transition: 180ms ease;
}

.toast.show {
  opacity: 1;
  transform: translateY(0);
}

.hidden {
  display: none !important;
}

@media (max-width: 780px) {
  .app {
    width: min(100% - 24px, 1120px);
  }

  .brand {
    padding: 17px 2px;
  }

  .brand-tag {
    display: none;
  }

  .hero {
    display: flex;
    min-height: auto;
    padding: 30px 4px 38px;
    flex-direction: column;
  }

  h1 {
    margin-top: 18px;
    font-size: clamp(3rem, 16vw, 4.6rem);
  }

  .pet-visual {
    width: 100%;
    min-height: 390px;
  }

  .yellow-disc {
    top: 30px;
    right: 10%;
    width: 310px;
  }

  .pet-card {
    width: 155px;
    height: 195px;
  }

  .pet-emoji {
    font-size: 4.6rem;
  }

  .dog-card {
    left: 2%;
  }

  .cat-card {
    right: 1%;
  }

  .gut-badge {
    right: 31%;
    bottom: 46px;
  }

  .home-benefits {
    grid-template-columns: 1fr;
  }

  .home-benefits article {
    padding: 22px 4px;
    border-right: 0;
    border-bottom: 1px solid var(--line);
  }

  .content-card,
  .quiz-card {
    padding: 26px 18px;
    border-radius: 22px;
  }

  .field-row {
    grid-template-columns: 1fr;
    gap: 0;
  }

  .quiz-card {
    min-height: 480px;
  }

  .result-top {
    padding-top: 24px;
  }

  .result-hero {
    grid-template-columns: 1fr;
    padding: 25px 20px;
    text-align: center;
  }

  .score-ring {
    width: 118px;
    height: 118px;
    margin: auto;
  }

  .report-grid {
    grid-template-columns: 1fr;
  }

  .advice-card {
    grid-column: auto;
  }
}

@media (max-width: 430px) {
  .pet-selector {
    grid-template-columns: 1fr;
  }

  .result-actions {
    grid-template-columns: 1fr;
  }

  footer {
    align-items: flex-start;
    flex-direction: column;
  }
}

@media print {
  body {
    background: white;
  }

  .brand,
  .small-button,
  .result-actions,
  footer,
  .sun-blob {
    display: none !important;
  }

  .app {
    width: 100%;
  }

  .screen {
    display: none !important;
  }

  #resultScreen {
    display: block !important;
  }

  .result-top {
    padding-top: 0;
  }

  .report-card,
  .result-hero,
  .medical-note {
    break-inside: avoid;
  }
}
