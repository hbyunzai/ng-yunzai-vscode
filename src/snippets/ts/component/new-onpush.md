---
description:
  zh-CN: OnPush 组件
  en-US: OnPush Component
---

```ts
import { ChangeDetectionStrategy, ChangeDetectorRef, Component, inject } from '@angular/core';
import { _HttpClient } from '@yelon/theme';

@Component({
  selector: 'app-${1}',
  templateUrl: './${1}.component.html',
  changeDetection: ChangeDetectionStrategy.OnPush,
})
export class ${1}Component {
  private readonly http = inject(_HttpClient);
  private readonly cdr = inject(ChangeDetectorRef);
}
```