![Static Badge](https://img.shields.io/badge/Alura-%230b182c)
![Static Badge](https://img.shields.io/badge/Django-4.2.13-%23092E20?logoColor=ffffff)

# Iniciar

```
cp .env.example .env
virtualenv venv
source venv/bin/activate
pip install -r requirements.txt
python manage.py collectstatic
python manage.py migrate
python manage.py createsuperuser
python manage.py runserver
```

# Passo a passo do curso

## 1 - Melhorias no projeto

Criar pasta **apps** e mover **galeria** e **usuarios** para ela.  
Mudaar as referencias ddos arquivos: **setup/settings.py**, **setup/urls.py**, **apps/galeria/apps.py**, **apps/galeria/admin.py**, **apps/galeria/urls.py**, **apps/galeria/views.py**, **apps/usuario/apps.py**, **apps/usuario/urls.py**, **apps/usuario/views.py**

## 2 - Inserir fotografias

Alterar arquivo **apps/galeria/urls.py** e **apps/galeria/views.py** adicionando opções de **nova, alterar e excluir**  
Alterar arquivo **templates/partials/_menu.html** adicionando opção de **nova imagem**  
Criar arquivo **templates/galeria/nova_imagem.html**

### Criar um formulário a partir de uma model

Criar arquivo **apps/galeria/forms.py**

