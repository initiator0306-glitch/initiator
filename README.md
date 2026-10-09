# initiator 웹사이트 초안

한국어/영어 전환, 모바일 대응, 외부 라이브러리 없는 정적 회사소개 사이트입니다.
브랜드명은 사용자가 확인한 initiator입니다. 현재 공개 배포 및 도메인 연결은 수행되지 않았습니다.

## 공개 전 입력할 실제 정보
- 정식 상호, 설립연도, 대표자, 공개할 사업장 정보
- 실제 취급 품목과 거래 국가, 실제 제공 서비스
- 문의 이메일: initiator@ditto3333.com (메일 수신 테스트 필요)
- Claude 활용 계획: 홍보, 제품 구매 프로토콜, 제품관리, 고객관리, 홈페이지 운영 체계. 사이트에는 도입 계획으로 표시했습니다.

## GitHub Pages 연결
1. GitHub에서 public 저장소 ditto-website를 만듭니다.
2. 이 폴더 안의 index.html, favicon.svg, CNAME, .nojekyll을 저장소 최상단에 업로드합니다. ZIP 파일 자체를 올리는 것이 아닙니다.
3. Settings → Pages → Build and deployment → Deploy from a branch → main / (root) → Save.
4. Custom domain에 ditto3333.com을 입력해 저장합니다.
5. GitHub 계정 Settings → Pages에서 도메인 소유권 인증을 진행하고 안내된 TXT 레코드를 DNS에 추가합니다.
6. 도메인의 DNS 관리에서 아래 A 레코드 4개를 입력합니다. 기존 웹사이트용 @ 레코드가 있다면 기존 운영 여부를 확인하고 교체합니다. 이메일용 MX/TXT는 보존합니다.

| 종류 | 호스트 | 값 |
|---|---|---|
| A | @ | 185.199.108.153 |
| A | @ | 185.199.109.153 |
| A | @ | 185.199.110.153 |
| A | @ | 185.199.111.153 |
| CNAME | www | 실제 GitHub아이디.github.io |

www의 값에는 저장소 이름을 붙이지 않습니다. www 연결은 선택사항입니다.
7. DNS 확인 및 인증서 발급 후 Enforce HTTPS를 켭니다.
8. https://ditto3333.com 에서 모바일 화면, 언어 전환, 각 메뉴, 실제 연락처를 확인합니다.
GitHub Pages는 이메일을 제공하지 않으므로 도메인 이메일은 별도 메일 서비스에서 설정해야 합니다.
현재 사이트에는 문의 전송 기능, AI API 연동, 결제, 방문자 추적이 없습니다.

## Claude 신청 준비
웹사이트만으로 승인이 보장되지 않습니다. 실제 사업 설명과 Claude 사용 목적을 일치시켜 신청하세요.
공식 페이지 확인일: 2026-10-09. Team 1년 무료 및 API 크레딧 1,000달러 제안은 현재 수용 한도 초과 안내가 있으므로 신청 직전에 확인하세요.
실제 검토할 수 있는 활용 예: 해외 거래처 이메일 번역·초안, 상품 사양 정리, 견적 조건 비교. 사용자가 확인한 활용 목적을 사이트의 도입 계획 섹션에 반영했습니다.

참고:
https://claude.com/programs/startups
https://www.anthropic.com/startup-program-official-terms
https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site
https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/verifying-your-custom-domain-for-github-pages

## Namecheap DNS 설정
Namecheap 로그인 → Domain List → ditto3333.com의 Manage → Advanced DNS → Host Records → Add New Record.
위 표의 A Record 4개와 선택사항인 www CNAME Record를 입력하고 TTL은 Automatic으로 설정합니다.
네임서버가 다른 DNS 제공업체를 가리키면 해당 업체에서 DNS를 변경해야 합니다. 네임서버를 임의로 바꾸지 마세요.
Namecheap 기본 주차용 www CNAME 또는 @ URL Redirect가 있으면 기존 사이트 운영 여부를 확인한 뒤 교체합니다.
initiator@ditto3333.com의 기존 MX 및 메일용 TXT 레코드는 보존하세요. 웹사이트 연결과 이메일 수신 설정은 별개입니다.
https://www.namecheap.com/support/knowledgebase/article.aspx/9645/2208/how-do-i-link-my-domain-to-github-pages/

## 운영 범위
이 파일은 정적 회사소개 초안입니다. 제품·고객 관리 시스템 및 AI 실행 기능은 포함하지 않습니다.
GitHub Pages는 상거래 및 상용 SaaS를 주목적으로 하는 사이트 운영에 제한이 있습니다. 실제 쇼핑·주문·결제 또는 고객관리 시스템을 구축할 경우 GitHub는 소스 관리에 사용하고, 호스팅은 별도 서비스를 선택하세요.
https://docs.github.com/en/pages/getting-started-with-github-pages/github-pages-limits

## Claude 신청 사업 설명 초안
initiator is an overseas wholesale, retail and international trade business. We plan to use Claude to draft and review marketing content, standardize product purchasing protocols, organize product information, develop customer inquiry response guidelines, and establish website content maintenance procedures. These are planned internal workflows, with human review before business decisions and publication.

이 문장은 사업 및 활용 계획 설명입니다. 설립연도, 실적, 투자 여부, 현재 구현 단계 등 신청서의 나머지 항목은 실제 정보로 작성해야 합니다.
