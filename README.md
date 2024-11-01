# LR6
Лабораторная работа №6

## Настройка

1. Аккаунт на Github был создан 5+ лет назад
2. Форк

![fork.png](imgs%2Ffork.png)

3. Git был скачан 5+ лет назад
4. Установка имени была проведена после клонирования репозитория, чтобы не изменять глобальный конфиг.
За все время пользования виндой, я так и не понял, какую кодировку нужно ставить... ни одна не работает. Но настройка прошла успешно!

![name.png](imgs%2Fname.png)

5. Клонирование

![clone.png](imgs%2Fclone.png)

## Веб интерфейс
6. Добавление файла через GitHub

![web_1.png](imgs%2Fweb_1.png)

![web_2.png](imgs%2Fweb_2.png)

## Локальная работа

7. История операций всех веток

![history_all.png](imgs%2Fhistory_all.png)

8. Все локальные изменения на момент скриншота

![local_changes.png](imgs%2Flocal_changes.png)

9. Merge через JetBrains IDEA. Второй скрин можно было и обрезать... 

![merge_1.png](imgs%2Fmerge_1.png)
![merge_2.png](imgs%2Fmerge_2.png)

10. Удаление ветки

![delete.png](imgs%2Fdelete.png)

11. Несколько изменений

![some_changes.png](imgs%2Fsome_changes.png)

12. Откат последнего коммита

![revert.png](imgs%2Frevert.png)

13. Ветка для отчета

![create_branch.png](imgs%2Fcreate_branch.png)

## Финальные штрихи

14. Оформление отчета (в процессе)

![img_1.png](imgs/report.png)

15. Красивая история операций

![pretty.png](imgs%2Fpretty.png)

16. git push. Вначале текущую ветку (report), потом все ветки.

![push_1.png](imgs%2Fpush_1.png)
![push_all.png](imgs%2Fpush_all.png)

## Лог комманд
Собран после выполнения ЛР. Может отсутствовать несколько команд :(

```bash
git clone https://github.com/thatusualguy/LR6
cd LR6
git log --all
git diff b4a235d7b4d26b38e500f9b40d698dfe5ecc6a7b
git branch -d branch1
git add -A
git commit -m "Небольшие изменения"
git add -A
git diff HEAD
git commit -m "Большие изменения"
git diff HEAD~1
git branch report
git checkout report
git log --pretty=format:"%h + %cd + %an + %s"
git push --all
git push origin -d branch1
doskey /history > commands.log # выгрузка истории команд из CMD
```