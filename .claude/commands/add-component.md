---
description: React 함수형 컴포넌트 파일을 src/components/ 폴더에 생성합니다
argument-hint: <ComponentName>
---

`$ARGUMENTS`를 컴포넌트 이름으로 사용하여 `src/components/$ARGUMENTS.tsx` 파일을 생성해줘.

파일 내용은 아래 템플릿을 따라야 해:

```tsx
import React from 'react'

interface ${ComponentName}Props {
  // props 정의
}

export default function ${ComponentName}({ }: ${ComponentName}Props) {
  return (
    <div className="">
      {/* 컴포넌트 내용 */}
    </div>
  )
}
```

규칙:
- 컴포넌트 이름은 `$ARGUMENTS` 그대로 사용 (PascalCase 유지)
- TypeScript interface로 Props 타입 정의
- Tailwind CSS className 사용
- `src/components/` 폴더에 `$ARGUMENTS.tsx`로 저장
- 파일이 이미 존재하면 덮어쓰지 말고 사용자에게 알려줘
