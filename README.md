���: ��django���һ�����׵�webƽ̨���������Զ������ԣ��ʺϳ�ѧ��ʹ��

���л��� linux python2.7 
1���޸����ݿ����� vim mysite_login/settings.py

DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': 'mysite_login',        
        'USER': 'root',          
        'PASSWORD': 'youpasswd',      #you mysql passwd
        'HOST': 'xxx',    #you mysql server ip
        'PORT': '3306',                   #
        }
2��pip install django 
3��pip install django-simple-captcha
4��pip install django-tinymce==2.4.0
5��pip install django-pure-pagination
6��pip install django-contrib-comments
7��pip install fields
8��Django 1.11����������-�޷���������Flatatt  ������޸�Դ��  �������һ�е����Ϊ:from django.forms.utils import flatatt 
9�����ݿ� mysite_login ��ҪΪutf-8 
 ���ߣ�alter database mysite_login character set utf8;
10��pip install pymysql
11��python manage.py makemigrations     
12��python manage.py migrate
13������
 python mange.py runserver 0.0.0.0:8000  
14������
 http://ip:8000/index/