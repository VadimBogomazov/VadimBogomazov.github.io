---
layout: default
title: Сниппеты
permalink: /snippets/

categories:
  - name: JS
    list:
        - name: Вычисление ширины скроллбара
          url: https://gist.github.com/vadimbogomazov/3718dea866e166092c5b6eb406f25baa
        - name: Cклонение слов
          url: https://gist.github.com/vadimbogomazov/0b3780160cb98b66e6187e5829f9636d
        - name: Случайное целое число&nbsp;от {min} до&nbsp;{max} включительно
          url: https://gist.github.com/vadimbogomazov/52358ec68dfa4341e3fb9d8cccad700b
  - name: CSS
    list:
        - name: visually-hidden
          url: https://gist.github.com/vadimbogomazov/ae41f882128c1afdd34c06d5bf6cacef
  - name: Миксины
    list:
        - name: font-face
          url: https://gist.github.com/vadimbogomazov/56d1bcc13c5d1cacbf1dfd88d8bf2a4b
        - name: Медиа-запросы для iPhone
          url: https://gist.github.com/vadimbogomazov/f0b8861804ce5fd4673310fec8f81a6a
  - name: HTML
    list:
        - name: Отключить преобразование телефонных номеров в&nbsp;ссылки в&nbsp;мобильных браузерах
          url: https://gist.github.com/vadimbogomazov/e5591be170a5f9318a672087f6363549
---

<p class="mt-0">Часто используемые сниппеты в&nbsp;работе, лежат на&nbsp;<a href="https://gist.github.com/vadimbogomazov" rel="noopener noreferrer" target="_blank">Github Gist</a>.</p>

<div>
    {% for category in page.categories %}
        <section class="site-section">
            <h2>{{ category.name }}</h2>

            <ul class="list">
                {% for item in category.list %}
                <li>
                    <a href="{{ item.url }}" rel="noopener noreferrer" target="_blank">{{ item.name }}</a>
                </li>
                {% endfor %}
            </ul>
        </section>
    {% endfor %}
</div>
