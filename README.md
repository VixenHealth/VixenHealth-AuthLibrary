# Сборка AuthLibrary

1. Создать wheel

```bash
python setup.py bdist_wheel
```

2. 1. Если вы хотите разрабатывать что-то с этой библиотекой - дополнительно запустите 
```bash
pip install dist/jwt_auth-1.0.0-py3-none-any.whl --force-reinstall
```

3. Вы прекрасны

Установка:
```bash
pip install git+https://github.com/VixenHealth/VixenHealth-AuthLibrary.git@master
```

> Важно отметить, что при редактировании библиотеки нужно использовать relative imports.

> Важно отметить #2
>
> Если вы меняете название\версию - нужно изменить Dockerfile. Там захардкожен путь.

> Важно отметить #3
>
> Специально для доклада сделал wheel, чтобы вы могли установить эту библиотеку в какой-нибудь проект и поиграться с
> ней.
