
<div align="center">

# 🚀 Libft

**Libft**는 C 표준 라이브러리의 주요 함수들을 직접 구현하여  
나만의 정적 라이브러리(`libft.a`)로 만드는 42서울의 필수 프로젝트입니다.  
이 라이브러리는 이후의 모든 42 프로젝트에서 재사용할 수 있으며,  
C 언어의 기본기를 탄탄히 다지는 데 필수적인 과제입니다.
<br>
이 과제는 https://velog.io/@cheringring/Libft 에 정리 해놓았습니다.

</div>

---

## 📝 프로젝트 개요

- **목표:**  
  C 표준 함수 및 추가 유틸리티 함수를 직접 구현하여,  
  다양한 프로젝트에서 활용 가능한 나만의 라이브러리 생성

- **출력물:**  
  - 정적 라이브러리 파일: `libft.a`
  - 헤더 파일: `libft.h`
  - 소스 파일: `ft_*.c`
  - Makefile

---

## 📂 디렉토리 구조

```
libft/
├── ft_*.c          # 구현 함수 소스 파일 
├── ft__*_bonus.c    # 보너스 구현 함수 소스 파일
├── libft.h        # 라이브러리 헤더
├── Makefile       # 빌드/정리/보너스 관리
└── README.md      # 프로젝트 설명 (본 파일)
```

---

## ⚙️ 개발 환경 및 빌드

- **언어:** C (C99 이하, restrict 사용 금지)
- **컴파일러:** cc
- **컴파일 플래그:** `-Wall -Wextra -Werror`
- **빌드 도구:** Makefile (필수)

### 빌드 명령어

| 명령어         | 설명                           |
| -------------- | ------------------------------ |
| `make`         | 라이브러리 빌드                |
| `make all`     | 라이브러리 빌드                |
| `make clean`   | 오브젝트 파일 삭제             |
| `make fclean`  | 오브젝트 + 라이브러리 삭제     |
| `make re`      | 전체 재빌드                    |
| `make bonus`   | 보너스 함수 포함 빌드          |

---

## 🛠️ 구현 함수 목록

<details>
<summary><b>1. 필수 함수 (Libc 함수 재구현)</b></summary>

- **문자/숫자 판별:**  
  `ft_isalpha`, `ft_isdigit`, `ft_isalnum`, `ft_isascii`, `ft_isprint`
- **문자열/메모리:**  
  `ft_strlen`, `ft_memset`, `ft_bzero`, `ft_memcpy`, `ft_memmove`  
  `ft_strlcpy`, `ft_strlcat`, `ft_strchr`, `ft_strrchr`, `ft_strncmp`  
  `ft_memchr`, `ft_memcmp`, `ft_strnstr`, `ft_strdup`
- **변환:**  
  `ft_toupper`, `ft_tolower`, `ft_atoi`
- **메모리 동적 할당:**  
  `ft_calloc`, `ft_strdup`

</details>

<details>
<summary><b>2. 추가 함수</b></summary>

- **문자열 처리:**  
  `ft_substr`, `ft_strjoin`, `ft_strtrim`, `ft_split`
- **변환:**  
  `ft_itoa`
- **함수형 프로그래밍:**  
  `ft_strmapi`, `ft_striteri`
- **파일 디스크립터 출력:**  
  `ft_putchar_fd`, `ft_putstr_fd`, `ft_putendl_fd`, `ft_putnbr_fd`

</details>

<details>
<summary><b>3. 보너스 함수 (연결 리스트)</b></summary>

- **리스트 생성/관리:**  
  `ft_lstnew`, `ft_lstadd_front`, `ft_lstsize`, `ft_lstlast`,  
  `ft_lstadd_back`, `ft_lstdelone`, `ft_lstclear`,  
  `ft_lstiter`, `ft_lstmap`

- **리스트 노드 구조체:**

typedef struct s_list
{
void *content;
struct s_list *next;
} t_list;

</details>

---

## 📑 주요 규칙 및 주의사항

- **Norminette(코딩 규칙) 필수 준수**
- **글로벌 변수 사용 금지**
- **메모리 누수 및 잘못된 해제 금지**
- **모든 소스는 루트(libft/)에 위치**
- **Makefile은 relink 금지, 필수 규칙 포함**
- **보너스는 별도 파일(_bonus.c/h)로 관리**

---

## 🧪 테스트

- 제출/평가 대상은 아니지만, 본인과 동료의 테스트 프로그램 제작을 권장합니다.
- 테스트 코드를 활용해 함수 동작, 예외 처리, 메모리 누수 등을 검증하세요.

---

## 💾 제출 및 평가

- **깃 저장소에 모든 파일 업로드**
- **파일명, 함수명, 규칙 정확히 준수**
- **평가 시, 제출된 저장소만 채점**

---

## 📜 라이선스 및 참고

- 본 프로젝트는 42서울 학습 목적으로 작성되었습니다.
- 직접 구현한 코드만 포함되어야 하며, 외부 코드 무단 사용은 금지됩니다.

---

<div align="center">

✨ Libft ✨

</div>
