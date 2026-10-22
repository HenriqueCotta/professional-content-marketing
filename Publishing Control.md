---
created_at:
updated_at: 2026-10-21
---

# Publishing Control

```base
filters:
  and:
    - file.ext == "md"
    - file.folder == this.file.path.replace(/[^/]+$/, "") + "Posts/" + file.basename
    - queue_order.isType("number")
    - queue_order >= 1
    - queue_order == queue_order.floor()
properties:
  file.name:
    displayName: Post
  note.queue_order:
    displayName: Posição
  note.post_status:
    displayName: Estado
views:
  - type: table
    name: Fila
    filters:
      and:
        - '["draft", "review", "ready"].contains(post_status)'
    order:
      - queue_order
      - file.name
      - post_status
    sort:
      - property: queue_order
        direction: ASC
      - property: post_status
        direction: ASC

```
