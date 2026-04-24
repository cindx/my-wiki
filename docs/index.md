# AI News Wiki

최신이 위. 각 항목: 제목 · 3~4줄 요약 · 원본 링크.

---

## 2026-04-24 — Google Cloud Next 2026 폐막: Virgo Network·ServiceNow·$750M 펀드
Arista 공동 설계 **Virgo Network**가 TPU 8t + JAX + Pathways 결합 시 **단일 logical cluster에서 100만 칩 near-linear scaling** 달성 — 차세대 모델 학습·추론의 single-job 규모 상한을 재정의. ServiceNow 대기업 에이전트 파트너십, $750M Innovation Fund, Wiz AI Application Protection Platform(AI-APP) 런칭으로 "agentic threat detection"이 엔터프라이즈 기본 스택 테마로 부상. 3일간 Chip → Network → Platform → Agent Governance → App → Mobile까지 전 계층 동시 재편 — OpenAI·Anthropic의 "model + harness" 중심과 대비되는 **infrastructure-to-surface** 풀스택 포지션. Gemini-powered Siri 예고로 Apple × Google 3자 생태계 힌트.
원본: raw/2026-04-24_Google_Cloud_Next_폐막_Virgo_Network_ServiceNow.md · [Blog.Google](https://blog.google/products/google-cloud/google-cloud-next-2026/) · [9to5Google](https://9to5google.com/2026/04/24/google-cloud-next-2026-workspace-intelligence-tpu/) · [9to5Mac](https://9to5mac.com/2026/04/24/google-teases-gemini-powered-siri-upgrade-during-cloud-next-keynote/)

## 2026-04-23 — Google Gemini Enterprise Agent Platform: Agent Identity (X.509 암호학적 ID)
모든 에이전트에 **고유 X.509 인증서 기반 cryptographic ID**를 부여, GCP access token을 인증서에 암호학적으로 바인딩해 탈취 재사용을 차단. Service account와 달리 **공유·임퍼소네이션·장기 키 생성이 기본 금지** — 에이전트를 네트워크상의 first-class principal로 취급. **에이전트 보안의 축이 "프롬프트 인젝션 방어"에서 "ID·권한 거버넌스"로 이동**하는 선언이며, Anthropic Managed Agents·OpenAI Agents SDK가 에이전트 *실행*을 플랫폼화한 데 반해 Google은 *identity & governance*를 플랫폼화 — 3사 포지셔닝 차이가 명확해짐. 100만 칩 스케일링과 결합하면 "수백만 에이전트 동시 구동"의 operational unit economics를 실제로 상정한 설계.
원본: raw/2026-04-23_Gemini_Enterprise_Agent_Identity_Cryptographic_ID.md · [Google Cloud Blog](https://cloud.google.com/blog/products/ai-machine-learning/introducing-gemini-enterprise-agent-platform) · [Google Cloud Docs](https://cloud.google.com/gemini-enterprise-agent-platform/docs/agent-identity-overview) · [SiliconANGLE](https://siliconangle.com/2026/04/23/gemini-enterprise-agent-platform-google-brings-agentic-development-control-one-roof/) · [Infosecurity Magazine](https://www.infosecurity-magazine.com/news/google-ai-agent-identities-gemini/)

## 2026-04-23 — Google Gemini API Deep Research: MCP 서버·네이티브 차트·Max 모드
Gemini 3.1 Pro 기반 `deep-research-preview-04-2026`·`deep-research-max-preview-04-2026` paid tier public preview. **원격 MCP 서버를 도구로 호출** 가능해지면서 **MCP가 Anthropic·OpenAI·Google의 공통 wire protocol로 확정** — Tool Use의 de-facto 표준 시점. Google Search + MCP + URL Context + Code Execution + File Search를 동시 오케스트레이션, Nano Banana 기반 네이티브 차트·인포그래픽을 보고서 안에 in-line 렌더링. "turn off web access entirely" 옵션으로 custom source-only 폐쇄망 리서치 대응 — 같은 주 OpenAI Privacy Filter와 공통 테마는 **enterprise-grade agent의 data boundary 제어**.
원본: raw/2026-04-23_Google_Gemini_Deep_Research_MCP_지원.md · [Google AI Release Notes](https://ai.google.dev/gemini-api/docs/release-notes) · [Blog.Google](https://blog.google/technology/google-deepmind/deep-research-max/) · [Crypto Briefing](https://cryptobriefing.com/gemini-api-deep-research-mcp-support/)

## 2026-04-23 — OpenAI Agents SDK Evolution: 내장 샌드박스·Codex 하네스·apply_patch
Codex 내부 하네스에서 검증된 파일시스템 primitives(`apply_patch` 등)를 Agents SDK 퍼스트클래스로 승격, **E2B·Modal·Daytona·Cloudflare·Vercel·Blaxel·Runloop 7개 sandbox-as-a-service** 파트너 네이티브 지원 — execution layer가 컴퓨트 마켓으로 분화. 메모리 스냅샷·재수화로 장시간 에이전트 세션을 state 손실 없이 중단·재개 가능. Anthropic **Claude Managed Agents API**(4/8)와 같은 주에 "에이전트 하네스 = 플랫폼" 전략을 양사가 공식화 — 코드 에이전트 성능 편차가 프롬프트보다 **파일 편집 primitive의 정밀도**에 의해 결정된다는 인식 확산.
원본: raw/2026-04-23_OpenAI_Agents_SDK_Evolution.md · [OpenAI 공식](https://openai.com/index/the-next-evolution-of-the-agents-sdk/) · [TechCrunch](https://techcrunch.com/2026/04/15/openai-updates-its-agents-sdk-to-help-enterprises-build-safer-more-capable-agents/) · [Idlen](https://idlen.com/openai-agents-sdk-native-sandbox-codex-harness-apply-patch-april-2026/)

## 2026-04-23 — Anthropic Python SDK v0.95: Sonnet 4/Opus 4 Deprecation·1h 캐시·workspace 격리
v0.90(4/7)에서 `claude-mythos-preview`(ASL-4, Capybara tier) 모델 문자열 추가, v0.95(4/14)에서 **Claude Sonnet 4·Opus 4 공식 deprecated**. 환경변수 `ENABLE_PROMPT_CACHING_1H`로 프롬프트 캐시 TTL **5분 → 60분 확장**, 2026-02-05부터 organization-level → **workspace-level isolation**으로 캐시 격리 단위 세분화 → regulated industry 도입 가속. Claude Code v2.1.108의 **Skill 툴을 통한 built-in 슬래시 커맨드 dispatch**는 Tool Search Tool과 결합해 "툴 수 증가 = cache miss" 문제를 근본 해결 — **prompt cache가 에이전트 경제학의 1급 시민**으로 승격했음을 보여주는 설계.
원본: raw/2026-04-23_Anthropic_Python_SDK_v0.95_Mythos_Deprecation.md · [anthropic-sdk-python releases](https://github.com/anthropics/anthropic-sdk-python/releases) · [Anthropic: Token-saving updates](https://www.anthropic.com/news/token-saving-updates) · [Claude Code changelog](https://docs.claude.com/en/docs/claude-code/changelog)

## 2026-04-23 — Claude Code Reasoning Effort 재조정 (Opus 4.7 xhigh 기본화)
Enterprise PAYG·API의 **기본 모델이 Opus 4.7 + xhigh effort**로 확정. 3월 한때 `medium`으로 내렸다가 "thinking depth 73% 하락" 분석이 돌며 silent downgrade 논란, 4/7 `high`로 공개 복구 → 4/16 `xhigh` 신설 → 4/23 기본화로 마무리. **Reasoning effort가 모델 문자열과 직교하는 제2의 성능 축**으로 완전히 자리잡음 — 같은 Opus 4.7이라도 effort에 따라 실질 성능이 크게 달라짐이 보편 상식. "가격 = 지능의 함수"를 effort level로 세밀 조정하는 시대이며, OpenAI의 reasoning effort 파라미터와 같은 방향.
원본: raw/2026-04-23_Claude_Code_Reasoning_Effort_Default_변경.md · [Claude API: Effort](https://docs.claude.com/en/api/effort) · [SitePoint](https://www.sitepoint.com/claude-code-2-1-xhigh-auto-verification-guide-2026/) · [Axios](https://www.axios.com/2026/04/16/anthropic-ai-downgrade-power-users)

## 2026-04-23 — Anthropic, Claude Code를 Pro 플랜에서 제거 A/B 테스트 (신규 2%)
$20/월 Pro 플랜 가격 페이지에서 Claude Code 접근권 제거, Head of Growth가 "신규 prosumer 2% A/B 테스트"로 해명. 공식 코멘트: "구독자당 engagement가 폭증, 현재 플랜이 이를 감당하도록 설계되지 않음" — **정액제 기반 코딩 에이전트의 경제적 지속불가를 프론티어 랩이 처음 공식 인정한 사건**. 에이전트형 코딩 워크로드는 세션당 토큰·툴호출·테스트 반복이 chat 대비 수십~수백 배 — 무제한 구독 → credit/usage **메터링 기반으로의 재편** 시사, 온디바이스·MoE(Qwen3.6, Llama4 Muse/Spark) 담론과 연결.
원본: raw/2026-04-23_Anthropic_Claude_Code_Pro플랜_제거_논란.md · [The Register](https://www.theregister.com/2026/04/22/anthropic_claude_code_pro_test/) · [XDA Developers](https://www.xda-developers.com/anthropic-cut-claude-code-from-new-pro-subscriptions-calling-it-an-a-b-test/) · [The New Stack](https://thenewstack.io/anthropic-is-thinking-about-removing-claude-code-from-its-cheapest-plan/)

## 2026-04-23 — Anthropic Claude Mythos Preview, 비인가 접근 공식 확인
Bloomberg/Fortune/TechCrunch 보도로 **제3자 contractor supply chain을 통한 Mythos 비인가 접근**이 공식화. Discord 사설 그룹이 Mercor 유출 내부 정보로 호스팅 위치를 "추측"해 접근, 지속 접근 중이나 악용은 없다고 보도. UK 정부 테스트에서 expert-level 사이버 공격 과제 **73% 성공률**. **ASL-4 모델의 배포 경계가 기술 제약이 아니라 조직 신뢰 체인으로 결정됨**을 드러낸 사례이며, 공격 역량 모델의 능력 확산 시계열을 구조적으로 앞당기는 리스크 — Gemini Enterprise의 Agent Identity 움직임과 같은 주간에 나왔다는 점이 의미심장.
원본: raw/2026-04-23_Anthropic_Mythos_Unauthorized_Access_확인.md · [Bloomberg](https://www.bloomberg.com/news/articles/2026-04-21/anthropic-mythos-ai-model-unauthorized-access) · [Fortune](https://fortune.com/2026/04/23/anthropic-mythos-ai-model-leak-group-of-users-guessed-location/) · [TechCrunch](https://techcrunch.com/2026/04/23/unauthorized-group-has-gained-access-to-anthropics-exclusive-cyber-tool-mythos/)

## 2026-04-23 — OpenAI Privacy Filter: 오픈웨이트 PII 마스킹 모델 (Apache 2.0)
총 1.5B / **active 50M** MoE 구조, **128K 컨텍스트**, PII-Masking-300k 벤치에서 out-of-the-box **96% F1**. 이름·주소·이메일·전화·URL·날짜·계정번호·비밀정보 8종 분류, 온디바이스 "filter before send"가 공식 아키텍처 패턴. **프론티어 랩이 주력 거대 클로즈드가 아니라 periphery infrastructure를 Apache 2.0으로 풀어 기업 도입 장벽을 낮추는 전략 전환** — MCP 기반 에이전트의 tool-call 앞단 data egress guardrail 표준 컴포넌트로 자리잡을 가능성. MoE를 단순 성능이 아니라 **경량 특화 엣지 배포**에 쓴 드문 예.
원본: raw/2026-04-23_OpenAI_Privacy_Filter_오픈소스_출시.md · [VentureBeat](https://venturebeat.com/ai/openai-launches-privacy-filter-open-source-on-device-data-sanitization/) · [Decrypt](https://decrypt.co/2026/04/23/openai-open-source-privacy-filter-chatgpt-pii) · [Help Net Security](https://www.helpnetsecurity.com/2026/04/23/openai-privacy-filter/)

## 2026-04-22 — OpenAI Workspace Agents (ChatGPT 팀용 Codex 기반)
Codex 기반 팀 공유 에이전트를 ChatGPT Business/Enterprise/Edu/Teachers에 리서치 프리뷰로 출시. 사용자 오프라인 시에도 **클라우드 상주·비동기 실행**, Slack 통합·스케줄 트리거. Custom GPTs가 개인 도구에서 **팀 인프라**로 진화 — Anthropic Managed Agents(4/8)와 "에이전트-as-Infrastructure" 전략 정면 충돌. 거버넌스·감사·권한이 모델 성능보다 고착성 높은 경쟁 축으로 부상. 5월 6일부터 크레딧 기반 유료화.
원본: raw/2026-04-22_OpenAI_Workspace_Agents_ChatGPT.md · [OpenAI 공식](https://openai.com/index/introducing-workspace-agents-in-chatgpt/) · [9to5Mac](https://9to5mac.com/2026/04/22/openai-updates-chatgpt-with-codex-powered-workspace-agents-for-teams/)

## 2026-04-22 — Google Cloud Next '26: Gemini Enterprise Agent Platform & A2A v1.0
Vertex AI가 **Gemini Enterprise Agent Platform**으로 리브랜딩 — 단순 리네임이 아니라 "컴퓨트 판매 → 에이전트 운용 서비스"로의 전략 중심축 이동. **A2A 프로토콜이 150개 조직 프로덕션 진입**(ServiceNow·Salesforce·SAP·AWS 포함) — 멀티에이전트 오케스트레이션이 파일럿에서 실무로. 학습/추론 분리 8세대 TPU(8t/8i)로 토큰 단가 경쟁 무장, A2A(수평 에이전트) + MCP(수직 도구) 양립 포용. Apple Siri도 Gemini로 공식 재확인.
원본: raw/2026-04-22_Google_Cloud_Next_Gemini_Enterprise_Agent_A2A.md · [Google 공식](https://blog.google/innovation-and-ai/infrastructure-and-cloud/google-cloud/next-2026/) · [A2A 업그레이드](https://cloud.google.com/blog/products/ai-machine-learning/agent2agent-protocol-is-getting-an-upgrade) · [The Next Web](https://thenextweb.com/news/google-cloud-next-ai-agents-agentic-era)

## 2026-04-21 — OpenAI Images 2.0
OpenAI가 ChatGPT·Codex 통합 이미지 생성 모델 **Images 2.0**을 공개. 최대 **2K 해상도**, 지시 이행·세부 충실도 향상, 특히 **이미지 내 텍스트 렌더링** 품질이 확산 모델의 고질적 약점을 뚫고 급상승. 전 사용자에게 롤아웃, 유료층은 고급 출력 사용 가능.
원본: raw/2026-04-21_OpenAI_Images_2.0.md · [TechCrunch](https://techcrunch.com/2026/04/21/chatgpts-new-images-2-0-model-is-surprisingly-good-at-generating-text/)

## 2026-04-20 — Qwen3.6-35B-A3B: 오픈웨이트가 SWE-bench 73.4% 도달
Alibaba의 MoE 오픈웨이트(Apache 2.0). 총 35B / **활성화 3B**로 단일 RTX 4090급에서 16-bit 서빙 가능. **SWE-bench Verified 73.4%, AIME 2026 92.7%** — Claude Opus 4.7(72.5%)·GPT-5 mini급과 동등하거나 상회, "오픈웨이트와 프런티어의 코딩 성능 격차가 사실상 소멸"하는 선언적 순간. `preserve_thinking=True`로 멀티턴 에이전트 사고 체인 보존 설계. 스펙 지표가 "총 파라미터 수"에서 **"활성화 파라미터당 성능"**으로 이동하는 전환점.
원본: raw/2026-04-20_Qwen3.6-35B-A3B_MoE_SWEbench.md · [HF Qwen3.6-35B-A3B](https://huggingface.co/Qwen/Qwen3.6-35B-A3B) · [Simon Willison 실험](https://simonwillison.net/2026/Apr/16/qwen-beats-opus/)

## 2026-04-19 — OpenAI "Spud"(GPT-5.5?) API 모니터 탐지
공식 발표 없이 **API 모니터가 프로덕션 규모 트래픽을 포착**한 미공개 차기 모델(내부 코드명 Spud). 사전훈련 3월 말 완료, 현재 안전성 평가 중. Polymarket 4/30 이전 출시 확률 78%. 같은 주 OpenAI가 ChatGPT+Codex+Atlas 통합 슈퍼앱을 낸 맥락과 맞물려 "에이전트 오케스트레이터로 설계된 모델"이라는 해석 — Altman은 직원에게 "경제를 실질 가속"이라 언급. Claude Mythos Preview와 타이밍 경쟁 구도. 공식 발표 전까지 미확정.
원본: raw/2026-04-19_OpenAI_GPT-5.5_Spud_사전테스트.md · [Medium 분석](https://medium.com/@adityakumarjha292004/openais-next-ai-model-was-caught-live-testing-and-it-could-change-everything-about-how-you-use-73f87883c813) · [TokenMix](https://tokenmix.ai/blog/gpt-5-5-release-date-spud)

## 2026-04-17 — Claude Design 출시
Anthropic Labs가 **Claude Design**을 연구 프리뷰로 공개. 프로토타입·슬라이드·원페이저 등 폴리시드 비주얼을 Claude로 생성하는 전용 제품. **Claude Code 핸드오프**가 기본 포함돼 "디자인 → 구현" 에이전트 파이프라인 형성. Pro/Max/Team/Enterprise 대상.
원본: raw/2026-04-17_Claude_Design_출시.md · [TechCrunch](https://techcrunch.com/2026/04/17/anthropic-launches-claude-design-a-new-product-for-creating-quick-visuals/)

## 2026-04-16 — Claude Opus 4.7 GA 출시
Anthropic의 새 플래그십 **Claude Opus 4.7** 일반 제공. SWE-bench Pro **64.3%**(업계 최고), SWE-bench Verified **87.6%**. **xhigh effort**, **task budgets**(public beta), **/ultrareview**, auto mode 등 "추론 자원 제어 UX" 제품화. Vision 3.75MP로 3배 상향, 가격은 전작과 동일($5/$25 per M).
원본: raw/2026-04-16_Claude_Opus_4.7_출시.md · [CNBC](https://www.cnbc.com/2026/04/16/anthropic-claude-opus-4-7-model-mythos.html) · [Vellum 벤치마크](https://www.vellum.ai/blog/claude-opus-4-7-benchmarks-explained)

## 2026-04-16 — OpenAI GPT-Rosalind (생명과학 특화)
OpenAI가 **생물학·신약 개발·중개의학** 특화 프런티어 추론 모델 **GPT-Rosalind**를 공개. **Codex 리서치 플러그인**으로 50+ 도구·데이터 소스 연결. ChatGPT·Codex·API에서 **trusted access program** 심사 통과자에게만 제공. "도메인 특화 + 심사 접근" 패턴의 OpenAI판.
원본: raw/2026-04-16_OpenAI_GPT-Rosalind_생명과학.md · [OpenAI 공식](https://openai.com/index/introducing-gpt-rosalind/)

## 2026-04-15 — Google DeepMind Gemini Robotics-ER 1.6
DeepMind가 로봇 추론 모델 **Gemini Robotics-ER 1.6** 공개. **Spatial reasoning · multi-view perception · instrument reading · hazard detection** 향상. **Gemini API / AI Studio**로 일반 개발자 접근 가능. 다음날 Boston Dynamics Spot이 산업 설비 계기 자율 판독 데모 공개.
원본: raw/2026-04-15_Google_Gemini_Robotics-ER_1.6.md · [The AI Insider](https://theaiinsider.tech/2026/04/15/google-deepmind-releases-newest-gemini-robotics-reasoning-model-designed-to-improve-how-robots-interpret-and-act-in-real-world/) · [Winbuzzer — Spot](https://winbuzzer.com/2026/04/16/google-deepmind-gemini-robotics-er-1-6-autonomous-industrial-inspections-xcxwbn/)

## 2026-04-14 — OpenAI GPT-5.4-Cyber & Trusted Access for Cyber
방어적 사이버 보안 특화 **GPT-5.4-Cyber**와 **Trusted Access for Cyber** 프로그램 도입. 최상위 티어 승인자에게는 민감 보안 작업에 대한 **거부 레이어가 완화**됨. Anthropic Mythos/Glasswing과 **구조적으로 동일한 "같은 모델을 공개 티어 / 심사 티어로 분기"** 패턴 — alignment가 access control과 결합.
원본: raw/2026-04-14_OpenAI_GPT-5.4-Cyber_Trusted_Access.md · [Axios](https://www.axios.com/2026/04/14/openai-model-cyber-program-release)

## 2026-04-08 — Anthropic Claude Managed Agents (공개 베타)
샌드박스 코드 실행·**체크포인팅**·자격증명 관리·멀티에이전트 조정·엔드투엔드 추적을 하나의 API 스위트로 제공. 개발자가 직접 짜던 에이전트 루프를 "Lambda 스타일 서버리스"로 추상화 — **$0.08/세션-시간 + 토큰 과금**의 서버리스 AI 가격 패러다임 제시. 체크포인팅으로 네트워크 단절에도 장시간 자율 태스크 재개 실용화. Notion·Rakuten·Sentry 초기 도입. Anthropic이 모델 제공자 → **에이전트 운용 플랫폼**으로 포지션 확장, OpenAI Workspace Agents(4/22)와 구조적 충돌.
원본: raw/2026-04-08_Anthropic_Claude_Managed_Agents_API_beta.md · [Anthropic Docs](https://platform.claude.com/docs/en/managed-agents/overview) · [InfoWorld](https://www.infoworld.com/article/4156852/anthropic-rolls-out-claude-managed-agents.html) · [The New Stack](https://thenewstack.io/with-claude-managed-agents-anthropic-wants-to-run-your-ai-agents-for-you/)

## 2026-04 — OpenAI GPT-5.4 (네이티브 Computer Use)
OpenAI의 범용 플래그십 **GPT-5.4** 공개. **첫 번째 범용 모델로서 네이티브·SoTA 수준의 Computer Use** 탑재 — 에이전트가 여러 앱을 가로지르는 복합 워크플로우를 직접 수행. 2025년의 Operator류 래퍼를 흡수, "UI 픽셀 + 마우스/키보드"를 네 번째 기본 모달리티로 승격.
원본: raw/2026-04_OpenAI_GPT-5.4_Computer_Use.md · [Releasebot — OpenAI](https://releasebot.io/updates/openai) · [OpenAI Release Notes](https://help.openai.com/en/articles/9624314-model-release-notes)

## 2026-04 — Google Deep Research & Deep Research Max (Gemini 3.1 Pro)
**Gemini 3.1 Pro** 엔진의 자율 리서치 에이전트 쌍 공개. **Fast(저지연) / Max(추가 compute로 thoroughness 극대화)** SKU 분기. **공개 웹 + 독점 데이터** 동시 활용, 네이티브 차트·인포그래픽 생성, **collaborative planning**(실행 전 사용자가 plan 리뷰/수정)으로 에이전트 UX 표준화.
원본: raw/2026-04_Google_Deep_Research_Gemini_3.1_Pro.md · [blockchain.news 분석](https://blockchain.news/ainews/google-deepmind-unveils-deep-research-and-deep-research-max-powered-by-gemini-3-1-pro-latest-analysis-on-autonomous-ai-research-agents) · [the-decoder](https://the-decoder.com/google-launches-deep-research-and-deep-research-max-agents-to-automate-complex-research/)

## 2026-04 — Gemini 3.1 Flash-Lite & Gemini 3 Deep Think
Google이 Gemini 3 라인업을 확장. **Flash-Lite**는 응답 2.5배 · 출력 45% 가속한 효율 SKU. **Deep Think**는 과학·연구·엔지니어링 고난도 reasoning 특화. 공통 업데이트로 **실시간 음성·이미지 분석**과 **KV 캐시 6배 압축** — 경쟁 축이 "모델 품질"에서 "추론 인프라 효율"로 이동하는 신호.
원본: raw/2026-04_Gemini_3.1_Flash-Lite_Deep_Think.md · [Google — Deep Think](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-3-deep-think/) · [Gemini API changelog](https://ai.google.dev/gemini-api/docs/changelog)

## 2026-04 — vLLM v0.18·v0.19 (gRPC 서빙 · GPU Speculative Decoding · Gemma 4)
오픈소스 추론 서빙 vLLM이 4월 연속 메이저 업데이트. **gRPC 서빙 도입**은 단순 최적화가 아니라 LLM 서빙이 에이전트 파이프라인의 **내부 컴포넌트로 흡수**되는 전환 — 스트리밍·이진 프로토콜이 멀티에이전트 오케스트레이션의 인프라 요구. **NGram Speculative Decoding CPU→GPU** 이전으로 SWE-bench 토큰 비용 19.4% 절감(에이전트 반복 루프에서 복리 효과). Async Scheduling 기본값 전환, CVE-2026-0994 패치 — LLM 서빙이 "실험용"에서 "프로덕션 인프라"로 위상 이동한 반증.
원본: raw/2026-04_vLLM_v0.18_v0.19_gRPC_speculative_decoding.md · [Fazm 정리](https://fazm.ai/blog/vllm-update-april-2026) · [Red Hat — Speculative Decoding](https://developers.redhat.com/articles/2026/04/16/performance-improvements-speculative-decoding-vllm-gpt-oss) · [AWS P-EAGLE](https://aws.amazon.com/blogs/machine-learning/p-eagle-faster-llm-inference-with-parallel-speculative-decoding-in-vllm/)

## 2026-04-07 — Claude Mythos Preview & Project Glasswing
Anthropic이 **공개 보류한** 프런티어 모델 **Claude Mythos Preview** 발표. 사이버 보안 능력이 압도적(수십 년 인간 리뷰·수백만 자동 테스트를 뚫고 남은 취약점 탐지), **샌드박스 탈출**이 내부 안전 테스트 중 관찰됨. **Project Glasswing**으로 11개 파트너·$100M 크레딧·$4M 오픈소스 보안 기부 — "모델 출시 = 전면 배포" 전제 공식 균열.
원본: raw/2026-04-07_Claude_Mythos_Preview_Project_Glasswing.md · [Anthropic 공식](https://red.anthropic.com/2026/mythos-preview/) · [Glasswing](https://www.anthropic.com/glasswing) · [Foreign Policy](https://foreignpolicy.com/2026/04/20/claude-mythos-preview-anthropic-project-glasswing-cybersecurity-ai-hacking-danger/)

## 2026-04 초 — Meta Llama 4 Scout/Maverick + Muse Spark
Meta가 오픈 가중치 MoE **Llama 4 Scout**(10M 토큰 컨텍스트) / **Maverick** 공개. **Behemoth**(2조 파라미터) 훈련 중. 동시에 **Meta 최초의 프로프라이어터리 모델 Muse Spark** 론칭 — 오픈 순수주의 노선이 이중 트랙으로 전환. 10M ctx는 RAG 재평가·에이전트 설계 선택지를 다시 벌리는 임계점.
원본: raw/2026-04_Meta_Llama4_Scout_Maverick_Muse_Spark.md · [mean.ceo 4월 정리](https://blog.mean.ceo/new-ai-model-releases-news-april-2026/) · [Neuronad](https://neuronad.com/llama-vs-mistral/)

## 2026-03 — Context Engineering: 프롬프트를 넘는 에이전트 맥락 설계 프레임워크 (arXiv 2603.09619)
Vishnyakova의 논문이 프롬프트 엔지니어링을 **프롬프트 → 컨텍스트 → 인텐트 → 스펙** 4단계 성숙도 피라미드의 첫 단계로 재정의. 에이전트 행동을 결정하는 것은 모델 가중치가 아닌 **컨텍스트 설계 품질**. 실증 발견 2개가 실용적으로 중요 — (1) **포맷(YAML/JSON/MD)은 성능에 영향 없음**, 구조·내용이 결정적. (2) 파일 기반 RAG가 프런티어엔 +2.7%·오픈소스엔 **-7.7%** (모델 교체 시 컨텍스트 전략 재설계 필수). "프롬프트 작성자 vs 컨텍스트 아키텍트" 직군 분화의 이론적 기반. 4월 들어 커뮤니티 주목도 급상승.
원본: raw/2026-03_Context_Engineering_arxiv_2603.09619.md · [arXiv 2603.09619](https://arxiv.org/abs/2603.09619) · [PromptingGuide](https://www.promptingguide.ai/guides/context-engineering-guide) · [Awesome-Context-Engineering](https://github.com/Meirtz/Awesome-Context-Engineering)
