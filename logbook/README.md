
<a name="readme-top"></a>


<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/karimFazlul/django-projects/tree/main/logbook">
    <img src="images/logo.png" alt="Logo" width="80" height="80">
  </a>


<h3 align="center">LogBook</h3>

  <p align="center">
   
   A blog system based on  <code> python3.8 </code> and <code>Django4.0</code>.

  </p>
</div>



<!-- TABLE OF CONTENTS -->

  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
		<li><a href="#built-with">Main Features</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Installation</a>
      <ul>
        <li><a href="#prerequisites">Configuration</a></li>
        <li><a href="#installation">Create database</a></li>
		<li><a href="#installation">Create Super User</a></li>
		<li><a href="#installation">Collect Static Files</a></li>
      </ul>
	  <li><a href="#installation">Run Server</a></li>
    </li>
    
  </ol>




<!-- ABOUT THE PROJECT -->
## About The Project





<p align="right">(<a href="#readme-top">back to top</a>)</p>



### Built With

* [![django][Django]][Django-url]
* [![postgreSQL][postgre]][postgre-url]
* [![HTML][html]][html-url]
* [![CSS][css]][css-url]
* [![JS][javascript]][js-url]
* [![Bootstrap][Bootstrap.com]][Bootstrap-url]
* [![JQuery][JQuery.com]][JQuery-url]

<p align="right">(<a href="#readme-top">back to top</a>)</p>









## Main Features:
- Posts, Pages, Categories, Tags(Add, Delete, Edit). Articles and pages support `Markdown`.
- Posts support **full-text search**.
- Complete comment feature, include posting reply comment. `Markdown` supporting.
- Post sharing through email.
- Sidebar feature: new articles, most readings, tags, etc.
- User Registration.
- User Login &  Logout.
- User Profile created automatically using signal.
- User Profile Edit.


## Installation:

Install via pip: 
```
pip install -Ur requirements.txt

```


### Configuration
Most configurations are in `setting.py`, others are in backend configurations.

I set many `setting` configuration with my environment variables (such as: `SECRET_KEY`, `OAUTH`, `postgreSQL` and some email configuration parts.) and they did NOT been submitted to the `GitHub`. You can change these in the code with your own configuration or just add them into your environment variables.



## Run

Modify `logbook/setting.py` with database settings, as following:

```python
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql',
        'NAME': 'DB_NAME',
        'USER': 'DB_USER',
        'PASSWORD': '******',
    }
}

```

### Create database


Run the following commands in Terminal:
```bash
python manage.py makemigrations
python manage.py migrate
```  

### Create super user

Run command in terminal:
```bash
python manage.py createsuperuser
```


### Collect static files
Run command in terminal:
```bash
python manage.py collectstatic --noinput
python manage.py compress --force
```

### Getting start to run server
Execute: `python manage.py runserver`

Open up a browser and visit: http://127.0.0.1:8000/ , the you will see the blog.
<p align="right">(<a href="#readme-top">back to top</a>)</p>











<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/github_username/repo_name.svg?style=for-the-badge
[contributors-url]: https://github.com/github_username/repo_name/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/github_username/repo_name.svg?style=for-the-badge
[forks-url]: https://github.com/github_username/repo_name/network/members
[stars-shield]: https://img.shields.io/github/stars/github_username/repo_name.svg?style=for-the-badge
[stars-url]: https://github.com/github_username/repo_name/stargazers
[issues-shield]: https://img.shields.io/github/issues/github_username/repo_name.svg?style=for-the-badge
[issues-url]: https://github.com/github_username/repo_name/issues
[license-shield]: https://img.shields.io/github/license/github_username/repo_name.svg?style=for-the-badge
[license-url]: https://github.com/github_username/repo_name/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/linkedin_username
[product-screenshot]: images/main-page.png
[Next.js]: https://img.shields.io/badge/next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white
[Next-url]: https://nextjs.org/
[React.js]: https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB
[React-url]: https://reactjs.org/
[Vue.js]: https://img.shields.io/badge/Vue.js-35495E?style=for-the-badge&logo=vuedotjs&logoColor=4FC08D
[Vue-url]: https://vuejs.org/
[Angular.io]: https://img.shields.io/badge/Angular-DD0031?style=for-the-badge&logo=angular&logoColor=white
[Angular-url]: https://angular.io/
[Svelte.dev]: https://img.shields.io/badge/Svelte-4A4A55?style=for-the-badge&logo=svelte&logoColor=FF3E00
[Svelte-url]: https://svelte.dev/
[Laravel.com]: https://img.shields.io/badge/Laravel-FF2D20?style=for-the-badge&logo=laravel&logoColor=white
[Laravel-url]: https://laravel.com
[Bootstrap.com]: https://img.shields.io/badge/Bootstrap-563D7C?style=for-the-badge&logo=bootstrap&logoColor=white
[Bootstrap-url]: https://getbootstrap.com
[JQuery.com]: https://img.shields.io/badge/jQuery-0769AD?style=for-the-badge&logo=jquery&logoColor=white
[JQuery-url]: https://jquery.com 
[Django]: https://img.shields.io/badge/django-0C4B33?style=for-the-badge&logo=django&logoColor=brightgreen
[Django-url]: https://www.djangoproject.com/
[html]: https://img.shields.io/badge/HTLM-35495E?style=for-the-badge&logo=html5&logoColor=
[html-url]:https://www.w3schools.com/html/
[css]:https://img.shields.io/badge/CSS-blue?style=for-the-badge&logo=css3&logoColor=
[css-url]:https://www.w3schools.com/css/
[javascript]:https://img.shields.io/badge/JavaScript-critical?style=for-the-badge&logo=javascript&logoColor=white
[js-url]:https://www.javascript.com/
[postgre]:https://img.shields.io/badge/postgresql-353044?style=for-the-badge&logo=postgresql&logoColor=
[postgre-url]:https://www.postgresql.org/
