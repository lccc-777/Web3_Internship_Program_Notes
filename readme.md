---
user:
    name: "cmu-ruoyan-lgl"
    age: 18
points:
    gather: 5
    eth_meeting: 10
    intern_meeting: 20
    intern_share: 40
    knowledge_live: 20
    knowledge_replay: 15
    notes: 10
---

这个项目是我用来完成Web3残酷共学签到创造的 记录学习笔记和任务证明，提醒每天的任务

### 常用link
- []

### 日常任务(完成后点击即可直接提交得分和任务证明):
- [ ] Gather Town晚自习（**5 分**）
- [ ] 参加以太坊中文周会（**10 分**）
- [ ] 参加周五实习计划例会（**20 分**）
- [ ] 参加周五实习计划例会并主动申请分享笔记或者感悟（**40 分**）
- [ ] 参加知识分享会（**20 分**）
- [ ] 未参加知识分享会，但是查看回放并且记录笔记（**15 分**）
- [ ] 整理一篇优秀学习笔记（**10 分**）

（**{{ page.user.name }} 分**）


- [ ] Gather Town 晚自习（**{{ page.points.gather }} 分**）
- [ ] 参加以太坊中文周会（**{{ page.points.eth_meeting }} 分**）
- [ ] 参加周五实习计划例会（**{{ page.points.intern_meeting }} 分**）
- [ ] 参加周五实习计划例会并主动申请分享笔记或者感悟（**{{ page.points.intern_share }} 分**）
- [ ] 参加知识分享会（**{{ page.points.knowledge_live }} 分**）
- [ ] 未参加知识分享会，但是查看回放并且记录笔记（**{{ page.points.knowledge_replay }} 分**）
- [ ] 整理一篇优秀学习笔记（**{{ page.points.notes }} 分**）这个只有上传到github后page.points.gather这些变量才能表现出具体数值吗