---
# 首页标题留空以使用站点标题
title: ''
summary: ''
date: 2022-10-24
type: landing

sections:
  - block: resume-biography-3
    content:
      # 选择要展示的作者档案（content/authors/ 下的文件夹名）
      username: me
      text: ''
      headings:
        about: '个人简介'
        education: ''
        interests: ''
    design:
      # 使用会自动适配主题配色的渐变网格背景
      background:
        gradient_mesh:
          enable: true

      # 姓名字号（适应长短姓名）
      name:
        size: md # 可选：xs, sm, md, lg（默认）, xl

      # 头像设置
      avatar:
        size: medium # 可选：small (150px), medium (200px，默认), large (320px), xl (400px), xxl (500px)
        shape: circle # 可选：circle（默认）, square, rounded
  - block: collection
    id: papers
    content:
      title: 出版物
      text: ''
      filters:
        folders:
          - publications
        exclude_featured: false
    design:
      view: citation
  - block: collection
    id: talks
    content:
      title: 报告
      filters:
        folders:
          - events
    design:
      view: card
  - block: collection
    id: popular-science
    content:
      title: 科普
      filters:
        folders:
          - popular-science
    design:
      view: card
  - block: collection
    id: news
    content:
      title: 最新博客
      subtitle: ''
      text: ''
      # 要展示的页面类型，例如 post、talk、publication……
      page_type: blog
      # 展示数量（0 表示全部）
      count: 10
      filters:
        author: ''
        category: ''
        tag: ''
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ''
      # 偏移量
      offset: 0
      # 排序方式：desc（降序）或 asc（升序）
      order: desc
    design:
      view: card
      spacing:
        padding: [0, 0, 0, 0]
  - block: cta-card
    demo: true # 仅在 HugoBlox Kit 演示站点显示
    content:
      title: 👉 像这样搭建你自己的学术网站
      text: |-
        本站由 HugoBlox Kit 生成——这是一个免费、基于 Hugo 的开源建站工具，已被 250,000+ 位学者使用。

        <a class="github-button" href="https://github.com/HugoBlox/kit" data-color-scheme="no-preference: light; light: light; dark: dark;" data-icon="octicon-star" data-size="large" data-show-count="true" aria-label="Star HugoBlox/kit on GitHub">Star</a>

        用区块搭建任何内容，无需写代码！

        从个人主页、第二大脑、课程到学术简历、会议与技术博客。
      button:
        text: 开始使用
        url: https://hugoblox.com/templates/
    design:
      card:
        css_class: 'bg-gradient-to-br from-primary-500 via-primary-600 to-secondary-600 text-white shadow-2xl'
        css_style: ''
---
