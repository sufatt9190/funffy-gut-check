const screens = [...document.querySelectorAll(".screen")];
const profileForm = document.querySelector("#profileForm");
const answerList = document.querySelector("#answerList");
const quizProgress = document.querySelector("#quizProgress");
const quizCount = document.querySelector("#quizCount");
const questionIcon = document.querySelector("#questionIcon");
const questionCategory = document.querySelector("#questionCategory");
const questionTitle = document.querySelector("#questionTitle");
const questionHelp = document.querySelector("#questionHelp");
const toast = document.querySelector("#toast");

const state = {
  profile: {},
  answers: {},
  questionIndex: 0,
};

const questions = [
  {
    id: "appetite",
    icon: "🍽️",
    category: "食欲",
    title: "过去 7 天，食欲有什么变化？",
    help: "请与平时正常状态比较。",
    options: [
      ["正常，和平时一样", 0],
      ["偶尔吃得少或挑食", 1],
      ["明显减少，常常吃不完", 2],
      ["几乎不吃或完全拒食", 3],
    ],
  },
  {
    id: "vomiting",
    icon: "💧",
    category: "呕吐",
    title: "过去 7 天，出现呕吐或干呕的频率？",
    help: "猫咪正常吐毛球也请计算在内。",
    options: [
      ["没有", 0],
      ["1 次", 1],
      ["2–3 次", 2],
      ["超过 3 次或一天多次", 3],
    ],
  },
  {
    id: "stool",
    icon: "💩",
    category: "排便",
    title: "最近的大便状态最接近哪一种？",
    help: "选择最近最常见或最严重的状态。",
    options: [
      ["成形、容易捡起", 0],
      ["偏软但仍有形状", 1],
      ["很软、糊状或偶尔水样", 2],
      ["持续水样腹泻或明显排便困难", 3],
    ],
  },
  {
    id: "frequency",
    icon: "🕒",
    category: "排便频率",
    title: "排便次数与平时相比如何？",
    help: "",
    options: [
      ["没有变化", 0],
      ["偶尔增加或减少", 1],
      ["明显变化，持续两天以上", 2],
      ["频繁急便、反复用力或超过一天未排便", 3],
    ],
  },
  {
    id: "energy",
    icon: "🎾",
    category: "精神与活动",
    title: "近期精神和活动力如何？",
    help: "",
    options: [
      ["活跃正常", 0],
      ["稍微懒散，但仍会玩", 1],
      ["明显没精神，不太愿意活动", 2],
      ["非常虚弱、站立困难或反应迟钝", 3],
    ],
  },
  {
    id: "weight",
    icon: "⚖️",
    category: "体重",
    title: "近期体重或体态有没有变化？",
    help: "若不确定，可以观察肋骨、腰线或抱起来的感觉。",
    options: [
      ["没有明显变化", 0],
      ["可能轻微下降", 1],
      ["看得出变瘦或体重持续下降", 2],
      ["短期内明显消瘦", 3],
    ],
  },
  {
    id: "duration",
    icon: "📅",
    category: "持续时间",
    title: "这些肠胃异常持续多久了？",
    help: "如果没有异常，请选择第一项。",
    options: [
      ["目前没有异常", 0],
      ["不到 24 小时", 1],
      ["2–3 天或反复出现", 2],
      ["超过 3 天或持续恶化", 3],
    ],
  },
  {
    id: "redFlags",
    icon: "🚨",
    category: "重要警示",
    title: "目前有没有以下任何一种情况？",
    help: "这一题不会加入普通分数，但会优先影响风险建议。",
    urgent: true,
    options: [
      ["以上都没有", 0, ""],
      ["呕吐物或粪便带血，或出现黑便", 0, "发现血便、黑便或呕吐物带血"],
      ["反复呕吐，连水也无法保留", 0, "反复呕吐且无法保留饮水"],
      ["腹部明显疼痛、鼓胀或持续蜷缩", 0, "出现明显腹痛或腹部鼓胀"],
      ["可能吞食异物、药物或有毒物质", 0, "可能吞食异物或有毒物质"],
      ["倒下、站立困难或反应异常", 0, "出现严重虚弱或反应异常"],
    ],
  },
];

const answerLabels = {
  appetite: ["食欲正常", "偶尔食欲下降", "食欲明显下降", "几乎或完全拒食"],
  vomiting: ["近期没有呕吐", "近期呕吐 1 次", "近期呕吐 2–3 次", "近期频繁呕吐"],
  stool: ["大便状态正常", "大便偏软", "大便糊状或偶尔水样", "持续腹泻或排便困难"],
  frequency: ["排便频率正常", "排便频率偶有变化", "排便频率明显改变", "频繁急便或长时间未排便"],
  energy: ["精神活动正常", "活动力稍有下降", "明显没精神", "严重虚弱"],
  weight: ["体重没有明显变化", "体重可能轻微下降", "出现明显变瘦", "短期内明显消瘦"],
  duration: ["目前没有异常", "异常不足 24 小时", "异常持续 2–3 天或反复", "异常超过 3 天或恶化"],
};

function showScreen(name) {
  screens.forEach((screen) => screen.classList.toggle("active", screen.dataset.screen === name));
  window.scrollTo({ top: 0, behavior: "smooth" });
  history.replaceState(null, "", `#${name}`);
}

function getSpeciesLabel() {
  return state.profile.species === "cat" ? "猫咪" : "狗狗";
}

function renderQuestion() {
  const question = questions[state.questionIndex];
  const quizNumber = state.questionIndex + 1;
  questionIcon.textContent = question.icon;
  questionCategory.textContent = question.category;
  questionTitle.textContent = question.title;
  questionHelp.textContent = question.help;
  quizCount.textContent = `${quizNumber} / ${questions.length}`;
  quizProgress.style.width = `${18 + (quizNumber / questions.length) * 68}%`;
  answerList.innerHTML = "";

  question.options.forEach(([label, score, reason], index) => {
    const button = document.createElement("button");
    button.type = "button";
    button.className = "answer-option";
    button.dataset.index = String(index);
    if (state.answers[question.id]?.index === index) button.classList.add("selected");
    button.innerHTML = `${label}<span>›</span>`;
    button.addEventListener("click", () => {
      state.answers[question.id] = { index, score, label, reason: reason || "" };
      button.classList.add("selected");
      window.setTimeout(() => {
        if (state.questionIndex < questions.length - 1) {
          state.questionIndex += 1;
          renderQuestion();
          window.scrollTo({ top: 0, behavior: "smooth" });
        } else {
          renderResult();
          showScreen("result");
        }
      }, 120);
    });
    answerList.appendChild(button);
  });
}

function calculateResult() {
  const score = questions
    .filter((question) => !question.urgent)
    .reduce((sum, question) => sum + (state.answers[question.id]?.score || 0), 0);
  const urgentReason = state.answers.redFlags?.reason || "";

  const catNotEating =
    state.profile.species === "cat" &&
    state.answers.appetite?.score === 3 &&
    state.answers.duration?.score >= 2;
  const vulnerable =
    ["young", "senior"].includes(state.profile.ageGroup) &&
    (state.answers.vomiting?.score >= 2 || state.answers.stool?.score >= 2);

  let risk = "low";
  if (score >= 15) risk = "high";
  else if (score >= 10) risk = "moderate";
  else if (score >= 5) risk = "watch";

  let overrideReason = urgentReason;
  if (catNotEating && !overrideReason) {
    overrideReason = "猫咪持续明显拒食并伴随多日异常";
  }
  if (vulnerable && risk === "low") risk = "watch";
  if (overrideReason) risk = "high";

  return { score, risk, urgentReason: overrideReason };
}

function riskContent(risk, hasUrgent) {
  const content = {
    low: {
      label: "较低风险",
      title: "目前整体表现较稳定",
      summary: "回答中暂未发现明显肠胃风险信号。继续维持稳定饮食，并留意日常食欲与排便变化。",
      advice: [
        "保持饮食稳定，避免突然换粮或一次给予过多新零食。",
        "继续观察未来 3–7 天的食欲、排便和精神状态。",
        "若出现新的异常或你仍感到担忧，可以咨询兽医。",
      ],
    },
    watch: {
      label: "需要观察",
      title: "出现一些轻微肠胃信号",
      summary: "目前有轻微或间歇性变化，建议更仔细记录饮食、呕吐与排便情况。",
      advice: [
        "记录未来 48 小时的进食量、饮水、呕吐和排便次数。",
        "避免突然换粮、油腻食物和不熟悉的零食。",
        "如果症状持续、反复或加重，请预约兽医检查。",
      ],
    },
    moderate: {
      label: "中度风险",
      title: "建议安排兽医评估",
      summary: "多个肠胃指标出现明显变化，仅凭线上测试无法确定原因，建议让兽医进一步检查。",
      advice: [
        "建议在近期联系兽医，并说明症状出现时间和变化趋势。",
        "保存粪便照片、呕吐次数和最近饮食记录，方便就诊说明。",
        "不要自行给予人用药物或未经兽医建议的止泻、止吐药。",
      ],
    },
    high: {
      label: hasUrgent ? "优先就医" : "较高风险",
      title: hasUrgent ? "建议尽快联系兽医" : "不建议继续单纯观察",
      summary: hasUrgent
        ? "回答中出现需要优先处理的警示信号。请尽快联系兽医或附近急诊动物医院。"
        : "症状分数较高或持续时间较长，建议尽快安排兽医检查。",
      advice: [
        "尽快联系执业兽医或附近动物医院，说明测试中出现的症状。",
        "若怀疑吞食异物或有毒物质，请保留包装或相关照片并立即求助。",
        "不要强行喂食、催吐或自行给予人用药物。",
      ],
    },
  };
  return content[risk];
}

function renderResult() {
  const { score, risk, urgentReason } = calculateResult();
  const content = riskContent(risk, Boolean(urgentReason));
  const date = new Intl.DateTimeFormat("zh-CN", {
    year: "numeric",
    month: "long",
    day: "numeric",
  }).format(new Date());

  document.querySelector("#resultPetName").textContent = state.profile.petName;
  document.querySelector("#resultDate").textContent = `测试日期：${date}`;
  document.querySelector("#scoreValue").textContent = score;
  document.querySelector("#riskLabel").textContent = content.label;
  document.querySelector("#riskTitle").textContent = content.title;
  document.querySelector("#riskSummary").textContent = content.summary;

  const hero = document.querySelector("#resultHero");
  hero.className = `result-hero ${risk}`;

  const urgentAlert = document.querySelector("#urgentAlert");
  urgentAlert.classList.toggle("hidden", !urgentReason);
  document.querySelector("#urgentReason").textContent = urgentReason
    ? `${urgentReason}。此类情况不应只依赖线上测试，请尽快寻求专业帮助。`
    : "";

  const ageLabels = { young: "1 岁以下", adult: "1–7 岁", senior: "8 岁以上" };
  const foodLabels = { no: "近期没有换粮", yes: "7 天内换过主食", unknown: "不确定" };
  document.querySelector("#profileSummary").innerHTML = `
    <div><dt>宠物</dt><dd>${escapeHtml(state.profile.petName)} · ${getSpeciesLabel()}</dd></div>
    <div><dt>年龄</dt><dd>${ageLabels[state.profile.ageGroup]}</dd></div>
    <div><dt>体重</dt><dd>${escapeHtml(state.profile.weight)} kg</dd></div>
    <div><dt>饮食变化</dt><dd>${foodLabels[state.profile.foodChange]}</dd></div>
    <div><dt>筛查得分</dt><dd>${score} / 21</dd></div>
  `;

  const findings = questions
    .filter((question) => !question.urgent)
    .map((question) => ({
      score: state.answers[question.id].score,
      label: answerLabels[question.id][state.answers[question.id].index],
    }))
    .filter((item) => item.score > 0)
    .sort((a, b) => b.score - a.score);

  document.querySelector("#findingList").innerHTML = (findings.length
    ? findings.slice(0, 5).map((item) => `<li>${escapeHtml(item.label)}</li>`)
    : ["目前各项回答均未显示明显异常"].map((item) => `<li>${item}</li>`)
  ).join("");

  document.querySelector("#adviceList").innerHTML = content.advice
    .map((item) => `<li>${escapeHtml(item)}</li>`)
    .join("");

  localStorage.setItem(
    "funffy-last-result",
    JSON.stringify({ profile: state.profile, answers: state.answers, score, risk, date })
  );
}

function escapeHtml(value) {
  const element = document.createElement("div");
  element.textContent = String(value);
  return element.innerHTML;
}

function restart() {
  state.profile = {};
  state.answers = {};
  state.questionIndex = 0;
  profileForm.reset();
  showScreen("home");
}

function showToast(message) {
  toast.textContent = message;
  toast.classList.add("show");
  clearTimeout(showToast.timer);
  showToast.timer = setTimeout(() => toast.classList.remove("show"), 1800);
}

document.querySelector("#startButton").addEventListener("click", () => showScreen("profile"));
document.querySelectorAll("[data-go]").forEach((button) => {
  button.addEventListener("click", () => showScreen(button.dataset.go));
});

profileForm.addEventListener("submit", (event) => {
  event.preventDefault();
  const data = new FormData(profileForm);
  state.profile = Object.fromEntries(data.entries());
  state.questionIndex = 0;
  renderQuestion();
  showScreen("quiz");
});

document.querySelector("#quizBackButton").addEventListener("click", () => {
  if (state.questionIndex === 0) {
    showScreen("profile");
    return;
  }
  state.questionIndex -= 1;
  renderQuestion();
});

document.querySelector("#restartButton").addEventListener("click", restart);
document.querySelector("#printButton").addEventListener("click", () => window.print());

document.querySelector("#shareButton").addEventListener("click", async () => {
  const { score, risk, urgentReason } = calculateResult();
  const content = riskContent(risk, Boolean(urgentReason));
  const text = [
    `🐾 ${state.profile.petName} 的 Funffy 肠胃健康测试`,
    `得分：${score}/21`,
    `风险等级：${content.label}`,
    content.title,
    "",
    "这是健康筛查结果，不替代兽医诊断。",
  ].join("\n");

  if (navigator.share) {
    try {
      await navigator.share({ title: "Funffy 肠胃健康测试", text });
    } catch (error) {
      if (error.name !== "AbortError") showToast("暂时无法分享");
    }
  } else {
    await navigator.clipboard.writeText(text);
    showToast("结果已复制，可以贴到 WhatsApp");
  }
});

if ("serviceWorker" in navigator && location.protocol.startsWith("http")) {
  navigator.serviceWorker.register("./sw.js").catch(() => {});
}

if (!["#profile", "#quiz", "#result"].includes(location.hash)) {
  showScreen("home");
}
