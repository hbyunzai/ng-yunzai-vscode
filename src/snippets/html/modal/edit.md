---
description:
  zh-CN: 模态框：编辑模式
  en-US: Modal edit mode demo
---

```html
<div class="modal-header">
  <div class="modal-title">$1</div>
</div>
<nz-spin *ngIf="!${2:i}" class="modal-spin"></nz-spin>
<sf *ngIf="$2" #sf mode="edit" [schema]="schema" [ui]="ui" [formData]="$2" button="none">
  <div class="modal-footer">
    <button nz-button type="button" (click)="close()">关闭</button>
    <button nz-button type="submit" [nzType]="'primary'" (click)="save(sf.value)" [disabled]="!sf.valid" [nzLoading]="http.loading">保存</button>
  </div>
</sf>
```