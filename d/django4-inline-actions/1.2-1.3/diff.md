# Comparing `tmp/django4-inline-actions-1.2.tar.gz` & `tmp/django4-inline-actions-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django4-inline-actions-1.2.tar", last modified: Mon Oct 31 15:12:12 2022, max compression
+gzip compressed data, was "django4-inline-actions-1.3.tar", last modified: Wed Apr 12 16:20:31 2023, max compression
```

## Comparing `django4-inline-actions-1.2.tar` & `django4-inline-actions-1.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2022-10-31 15:12:12.252471 django4-inline-actions-1.2/
--rw-rw-rw-   0        0        0     1537 2022-10-31 14:36:03.000000 django4-inline-actions-1.2/LICENSE
--rw-rw-rw-   0        0        0    17641 2022-10-31 15:12:12.253471 django4-inline-actions-1.2/PKG-INFO
--rw-rw-rw-   0        0        0    13130 2022-10-31 15:10:18.000000 django4-inline-actions-1.2/README.md
-drwxrwxrwx   0        0        0        0 2022-10-31 15:12:12.228031 django4-inline-actions-1.2/django4_inline_actions.egg-info/
--rw-rw-rw-   0        0        0    17641 2022-10-31 15:12:12.000000 django4-inline-actions-1.2/django4_inline_actions.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      854 2022-10-31 15:12:12.000000 django4-inline-actions-1.2/django4_inline_actions.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-31 15:12:12.000000 django4-inline-actions-1.2/django4_inline_actions.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-10-31 14:48:55.000000 django4-inline-actions-1.2/django4_inline_actions.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       25 2022-10-31 15:12:12.000000 django4-inline-actions-1.2/django4_inline_actions.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-10-31 15:12:12.231545 django4-inline-actions-1.2/inline_actions/
--rw-rw-rw-   0        0        0        0 2022-10-31 12:02:27.000000 django4-inline-actions-1.2/inline_actions/__init__.py
--rw-rw-rw-   0        0        0     1425 2022-10-31 12:02:27.000000 django4-inline-actions-1.2/inline_actions/actions.py
--rw-rw-rw-   0        0        0    10489 2022-10-31 12:02:27.000000 django4-inline-actions-1.2/inline_actions/admin.py
-drwxrwxrwx   0        0        0        0 2022-10-31 15:12:12.233548 django4-inline-actions-1.2/inline_actions/templatetags/
--rw-rw-rw-   0        0        0        0 2022-10-31 12:02:27.000000 django4-inline-actions-1.2/inline_actions/templatetags/__init__.py
--rw-rw-rw-   0        0        0      810 2022-10-31 12:02:27.000000 django4-inline-actions-1.2/inline_actions/templatetags/inline_action_tags.py
--rw-rw-rw-   0        0        0     2111 2022-10-31 15:12:05.000000 django4-inline-actions-1.2/pyproject.toml
--rw-rw-rw-   0        0        0      829 2022-10-31 15:12:12.254470 django4-inline-actions-1.2/setup.cfg
--rw-rw-rw-   0        0        0     2003 2022-10-31 15:12:06.000000 django4-inline-actions-1.2/setup.py
-drwxrwxrwx   0        0        0        0 2022-10-31 15:12:12.193059 django4-inline-actions-1.2/test_proj/
-drwxrwxrwx   0        0        0        0 2022-10-31 15:12:12.239545 django4-inline-actions-1.2/test_proj/blog/
--rw-rw-rw-   0        0        0        0 2022-10-31 12:02:27.000000 django4-inline-actions-1.2/test_proj/blog/__init__.py
--rw-rw-rw-   0        0        0     4480 2022-10-31 14:58:21.000000 django4-inline-actions-1.2/test_proj/blog/admin.py
--rw-rw-rw-   0        0        0      164 2022-10-31 12:02:27.000000 django4-inline-actions-1.2/test_proj/blog/forms.py
-drwxrwxrwx   0        0        0        0 2022-10-31 15:12:12.242953 django4-inline-actions-1.2/test_proj/blog/migrations/
--rw-rw-rw-   0        0        0     1652 2022-10-31 12:02:27.000000 django4-inline-actions-1.2/test_proj/blog/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2022-10-31 12:02:27.000000 django4-inline-actions-1.2/test_proj/blog/migrations/__init__.py
--rw-rw-rw-   0        0        0      783 2022-10-31 12:02:27.000000 django4-inline-actions-1.2/test_proj/blog/models.py
-drwxrwxrwx   0        0        0        0 2022-10-31 15:12:12.251469 django4-inline-actions-1.2/test_proj/blog/tests/
--rw-rw-rw-   0        0        0        0 2022-10-31 12:02:27.000000 django4-inline-actions-1.2/test_proj/blog/tests/__init__.py
--rw-rw-rw-   0        0        0     8292 2022-10-31 14:58:23.000000 django4-inline-actions-1.2/test_proj/blog/tests/test_admin.py
--rw-rw-rw-   0        0        0     1023 2022-10-31 12:02:27.000000 django4-inline-actions-1.2/test_proj/blog/tests/test_form.py
--rw-rw-rw-   0        0        0     7975 2022-10-31 14:58:23.000000 django4-inline-actions-1.2/test_proj/blog/tests/test_inline_admin.py
--rw-rw-rw-   0        0        0     5669 2022-10-31 14:58:24.000000 django4-inline-actions-1.2/test_proj/blog/tests/test_model_admin.py
--rw-rw-rw-   0        0        0     1345 2022-10-31 14:58:25.000000 django4-inline-actions-1.2/test_proj/blog/tests/test_templatetags.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:20:31.862683 django4-inline-actions-1.3/
+-rw-rw-rw-   0        0        0     1537 2022-10-31 14:36:03.000000 django4-inline-actions-1.3/LICENSE
+-rw-rw-rw-   0        0        0    14653 2023-04-12 16:20:31.862683 django4-inline-actions-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0    13204 2022-10-31 15:20:55.000000 django4-inline-actions-1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 16:20:31.806951 django4-inline-actions-1.3/django4_inline_actions.egg-info/
+-rw-rw-rw-   0        0        0    14653 2023-04-12 16:20:31.000000 django4-inline-actions-1.3/django4_inline_actions.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      854 2023-04-12 16:20:31.000000 django4-inline-actions-1.3/django4_inline_actions.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 16:20:31.000000 django4-inline-actions-1.3/django4_inline_actions.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-10-31 14:48:55.000000 django4-inline-actions-1.3/django4_inline_actions.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       25 2023-04-12 16:20:31.000000 django4-inline-actions-1.3/django4_inline_actions.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 16:20:31.814951 django4-inline-actions-1.3/inline_actions/
+-rw-rw-rw-   0        0        0        0 2022-10-31 12:02:27.000000 django4-inline-actions-1.3/inline_actions/__init__.py
+-rw-rw-rw-   0        0        0     1425 2022-10-31 12:02:27.000000 django4-inline-actions-1.3/inline_actions/actions.py
+-rw-rw-rw-   0        0        0    10489 2022-10-31 12:02:27.000000 django4-inline-actions-1.3/inline_actions/admin.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:20:31.818962 django4-inline-actions-1.3/inline_actions/templatetags/
+-rw-rw-rw-   0        0        0        0 2022-10-31 12:02:27.000000 django4-inline-actions-1.3/inline_actions/templatetags/__init__.py
+-rw-rw-rw-   0        0        0      810 2022-10-31 12:02:27.000000 django4-inline-actions-1.3/inline_actions/templatetags/inline_action_tags.py
+-rw-rw-rw-   0        0        0     2119 2023-04-12 16:18:27.000000 django4-inline-actions-1.3/pyproject.toml
+-rw-rw-rw-   0        0        0      829 2023-04-12 16:20:31.866679 django4-inline-actions-1.3/setup.cfg
+-rw-rw-rw-   0        0        0     2003 2023-04-12 16:20:29.000000 django4-inline-actions-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:20:31.777346 django4-inline-actions-1.3/test_proj/
+drwxrwxrwx   0        0        0        0 2023-04-12 16:20:31.832472 django4-inline-actions-1.3/test_proj/blog/
+-rw-rw-rw-   0        0        0        0 2022-10-31 12:02:27.000000 django4-inline-actions-1.3/test_proj/blog/__init__.py
+-rw-rw-rw-   0        0        0     4480 2022-10-31 14:58:21.000000 django4-inline-actions-1.3/test_proj/blog/admin.py
+-rw-rw-rw-   0        0        0      164 2022-10-31 12:02:27.000000 django4-inline-actions-1.3/test_proj/blog/forms.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:20:31.838480 django4-inline-actions-1.3/test_proj/blog/migrations/
+-rw-rw-rw-   0        0        0     1652 2022-10-31 12:02:27.000000 django4-inline-actions-1.3/test_proj/blog/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2022-10-31 12:02:27.000000 django4-inline-actions-1.3/test_proj/blog/migrations/__init__.py
+-rw-rw-rw-   0        0        0      783 2022-10-31 12:02:27.000000 django4-inline-actions-1.3/test_proj/blog/models.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:20:31.859682 django4-inline-actions-1.3/test_proj/blog/tests/
+-rw-rw-rw-   0        0        0        0 2022-10-31 12:02:27.000000 django4-inline-actions-1.3/test_proj/blog/tests/__init__.py
+-rw-rw-rw-   0        0        0     8292 2022-10-31 14:58:23.000000 django4-inline-actions-1.3/test_proj/blog/tests/test_admin.py
+-rw-rw-rw-   0        0        0     1023 2022-10-31 12:02:27.000000 django4-inline-actions-1.3/test_proj/blog/tests/test_form.py
+-rw-rw-rw-   0        0        0     7975 2022-10-31 14:58:23.000000 django4-inline-actions-1.3/test_proj/blog/tests/test_inline_admin.py
+-rw-rw-rw-   0        0        0     5669 2022-10-31 14:58:24.000000 django4-inline-actions-1.3/test_proj/blog/tests/test_model_admin.py
+-rw-rw-rw-   0        0        0     1345 2022-10-31 14:58:25.000000 django4-inline-actions-1.3/test_proj/blog/tests/test_templatetags.py
```

### Comparing `django4-inline-actions-1.2/LICENSE` & `django4-inline-actions-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django4-inline-actions-1.2/PKG-INFO` & `django4-inline-actions-1.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,408 +1,411 @@
 Metadata-Version: 2.1
 Name: django4-inline-actions
-Version: 1.2
+Version: 1.3
 Summary: django4-inline-actions adds actions to each row of the ModelAdmin or InlineModelAdmin
 Home-page: https://github.com/HiroshiFuu/django4-inline-actions
+Download-URL: https://pypi.python.org/pypi/django4-inline-actions
 Author: FENG Hao
 Author-email: hiroshifuu@outlook.com
 License: BSD
-Download-URL: https://pypi.python.org/pypi/django4-inline-actions
-Description: # django4-inline-actions
-        
-        ![PyPI](https://img.shields.io/pypi/v/django4-inline-actions?style=flat-square)
-        <!-- ![GitHub Workflow Status (master)](https://img.shields.io/github/workflow/status/HiroshiFuu/django4-inline-actions/Test%20&%20Lint/master?style=flat-square) -->
-        <!-- ![Coveralls github branch](https://img.shields.io/coveralls/github/HiroshiFuu/django4-inline-actions/master?style=flat-square) -->
-        ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django4-inline-actions?style=flat-square)
-        ![PyPI - License](https://img.shields.io/pypi/l/django4-inline-actions?style=flat-square)
-        
-        django4-inline-actions adds actions to each row of the ModelAdmin or InlineModelAdmin. Add support for Django 4.
-        
-        ## Requirements
-        
-        * Python 3.8 or newer
-        
-        ## Screenshot
-        
-        ![Changelist example](https://raw.githubusercontent.com/HiroshiFuu/django4-inline-actions/master/example_changelist.png)
-        ![Inline example](https://raw.githubusercontent.com/HiroshiFuu/django4-inline-actions/master/example_inline.png)
-        
-        ## Installation
-        
-        1. Install django4-inline-actions
-        
-           ```sh
-           pip install django4-inline-actions
-           ```
-        
-        2. Add `inline_actions` to your `INSTALLED_APPS`.
-        
-        ## Integration
-        
-        Add the `InlineActionsModelAdminMixin` to your `ModelAdmin`.
-        If you want to have actions on your inlines, add the `InlineActionsMixin` to your `InlineModelAdmin`.
-        Each action is implemented as a method on the `ModelAdmin`/`InlineModelAdmin` and **must have** the following signature.
-        
-        ```python
-        def action_name(self, request, obj, parent_obj=None):
-        ```
-        
-        | Argument     | Description                                       |
-        |--------------|---------------------------------------------------|
-        | `request`    | current request                                   |
-        | `obj`        | instance on which the action was triggered        |
-        | `parent_obj` | instance of the parent model, only set on inlines |
-        
-        and should return `None` to return to the current changeform or a `HttpResponse`.
-        Finally, add your method name to list of actions `inline_actions` defined on the corresponding `ModelAdmin`.
-        If you want to disable the *actions* column, you have to explicitly set `inline_actions = None`.
-        To add your actions dynamically, you can use the method `get_inline_actions(self, request, obj=None)` instead.
-        
-        This module is bundled with two actions for viewing (`inline_actions.actions.ViewAction`) and deleting (`inline_actions.actions.DeleteAction`).
-        Just add these classes to your admin and you're done.
-        
-        Additionally, you can add methods to generate a custom label and CSS classes per object.
-        If you have an inline action called `action_name` then you can define
-        
-        ```python
-        def get_action_name_label(self, obj):
-            return 'some string'
-        
-        def get_action_name_css(self, obj):
-            return 'some string'
-        ```
-        
-        | Argument | Description                                |
-        |----------|--------------------------------------------|
-        | `obj`    | instance on which the action was triggered |
-        
-        Each defined method has to return a string.
-        
-        ### Example 1
-        
-        Imagine a simple news application with the following `admin.py`.
-        
-        ```python
-        from django.contrib import admin
-        from inline_actions.admin import InlineActionsMixin
-        from inline_actions.admin import InlineActionsModelAdminMixin
-        
-        from .models import Article, Author
-        
-        
-        class ArticleInline(InlineActionsMixin,
-                            admin.TabularInline):
-            model = Article
-            inline_actions = []
-        
-            def has_add_permission(self, request, obj=None):
-                return False
-        
-        
-        @admin.register(Author)
-        class AuthorAdmin(InlineActionsModelAdminMixin,
-                          admin.ModelAdmin):
-            inlines = [ArticleInline]
-            list_display = ('name',)
-        
-        
-        @admin.register(Article)
-        class AuthorAdmin(admin.ModelAdmin):
-            list_display = ('title', 'status', 'author')
-        ```
-        
-        We now want to add two simple actions (`view`, `unpublish`) to each article within the `AuthorAdmin`.
-        The `view` action redirects to the changeform of the selected instance.
-        
-        ```python
-        from django.core.urlresolvers import reverse
-        from django.shortcuts import redirect
-        
-        
-        class ArticleInline(InlineActionsMixin,
-                            admin.TabularInline):
-            # ...
-            inline_actions = ['view']
-            # ...
-        
-            def view(self, request, obj, parent_obj=None):
-                url = reverse(
-                    'admin:{}_{}_change'.format(
-                        obj._meta.app_label,
-                        obj._meta.model_name,
-                    ),
-                    args=(obj.pk,)
-                )
-                return redirect(url)
-            view.short_description = _("View")
-        ```
-        
-        Since `unpublish` depends on `article.status` we must use `get_inline_actions` to add this action dynamically.
-        
-        ```python
-        from django.contrib import admin, messages
-        from django.utils.translation import gettext_lazy as _
-        
-        
-        class ArticleInline(InlineActionsMixin,
-                            admin.TabularInline):
-            # ...
-            def get_inline_actions(self, request, obj=None):
-                actions = super(ArticleInline, self).get_inline_actions(request, obj)
-                if obj:
-                    if obj.status == Article.PUBLISHED:
-                        actions.append('unpublish')
-                return actions
-        
-            def unpublish(self, request, obj, parent_obj=None):
-                obj.status = Article.DRAFT
-                obj.save()
-                messages.info(request, _("Article unpublished"))
-            unpublish.short_description = _("Unpublish")
-        ```
-        
-        Adding `inline_actions` to the changelist works similar. See the sample project for further details (`test_proj/blog/admin.py`).
-        
-        ### Example 2
-        
-        Instead of creating separate actions for publishing and unpublishing, we might prefer an action, which toggles between those two states.
-        `toggle_publish` implements the behaviour described above.
-        
-        ```python
-        def toggle_publish(self, request, obj, parent_obj=None):
-            if obj.status == Article.DRAFT:
-                obj.status = Article.PUBLISHED
-            else:
-                obj.status = Article.DRAFT
-        
-            obj.save()
-        
-            if obj.status == Article.DRAFT:
-                messages.info(request, _("Article unpublished."))
-            else:
-                messages.info(request, _("Article published."))
-        ```
-        
-        This might leave the user with an ambiguous button label as it will be called `Toggle publish` regardless of the internal state.
-        We can specify a dynamic label by adding a special method `get_ACTIONNAME_label`.
-        
-        ```python
-        def get_toggle_publish_label(self, obj):
-            if obj.status == Article.DRAFT:
-                return 'Publish'
-            return 'Unpublish'
-        ```
-        
-        So assuming an object in a row has `DRAFT` status, then the button label will be `Toggle publish` and `Toggle unpublish` otherwise.
-        
-        We can go even fancier when we create a method that will add css classes for each object depending on a status like:
-        
-        ```python
-        def get_toggle_publish_css(self, obj):
-            if obj.status == Article.DRAFT:
-                return 'btn-red'
-            return 'btn-green'
-        ```
-        
-        You can make it more eye-candy by using `btn-green` that makes your button green and `btn-red` that makes your button red.
-        Or you can use those classes to add some javascript logic (i.e. confirmation box).
-        
-        ### Tip on confirmation alerts
-        
-        When performing a certain critical action or ones which may not be easily reversible it's good to have a confirmation prompt before submitting the action form. To achieve this, one way would be to override `templates/admin/change_list.html` with the following.
-        
-        ```html
-        {% extends "admin/change_list.html" %}
-        
-        {% block extrahead %}
-            {{ block.super }}
-            <script>
-                (function() {
-                    document.addEventListener("DOMContentLoaded", function(event) {
-                        let inline_actions = document.querySelectorAll(".inline_actions input");
-                        for (var i=0; i < inline_actions.length; i++) {
-                            inline_actions[i].addEventListener("click", function(e) {
-                                if(!confirm("Do you really want to " + e.target.value + "?")) {
-                                    e.preventDefault();
-                                }
-                            });
-                        }
-                    });
-                })();
-            </script>
-        {% endblock %}
-        ```
-        
-        If a staff user has clicked any inline action accidentally, they can safely click no in the confirmation prompt & the inline action form would not be submitted.
-        
-        ## Intermediate forms
-        
-        The current implementation for using intermediate forms involves some manual handling.
-        This will be simplified in the next major release!
-        
-        
-        In order to have an intermediate form, you must add some information about the triggered action.
-        `django4-inline-actions` provides a handy templatetag `render_inline_action_fields`,
-        which adds these information as hidden fields to a form.
-        
-        ```html
-        {% extends "admin/base_site.html" %}
-        {% load inline_action_tags %}
-        
-        {% block content %}
-          <form action="" method="post">
-            {% csrf_token %}
-            {% render_inline_action_fields %}
-        
-            {{ form.as_p }}
-        
-            <input type="submit" name="_back" value="Cancel"/>
-            <input type="submit" name="_save" value="Update"/>
-          </form>
-        {% endblock %}
-        ```
-        
-        As the action does not know that an intermediate form is used, we have to include some special handling.
-        In the case above we have to consider 3 cases:
-        
-        1. The form has been submitted and we want to redirect to the previous view.
-        2. Back button has been clicked.
-        3. Initial access to the intermediate page/form.
-        
-        The corresponding action could look like
-        
-        ```python
-            def change_title(self, request, obj, parent_obj=None):
-        
-                # 1. has the form been submitted?
-                if '_save' in request.POST:
-                    form = forms.ChangeTitleForm(request.POST, instance=obj)
-                    form.save()
-                    return None  # return back to list view
-                # 2. has the back button been pressed?
-                elif '_back' in request.POST:
-                    return None  # return back to list view
-                # 3. simply display the form
-                else:
-                    form = forms.ChangeTitleForm(instance=obj)
-        
-                return render(
-                    request,
-                    'change_title.html',
-                    context={'form': form}
-                )
-        ```
-        
-        ## Example Application
-        
-        You can see `django4-inline-actions` in action using the bundled test application `test_proj`.
-        Use [`poetry`](https://poetry.eustace.io/) to run it.
-        
-        ```bash
-        git clone https://github.com/HiroshiFuu/django4-inline-actions.git
-        cd django4-inline-actions/
-        poetry install
-        poetry run pip install Django
-        cd test_proj
-        poetry run ./manage.py migrate
-        poetry run ./manage.py createsuperuser
-        poetry run ./manage.py runserver
-        ```
-        
-        Open [`http://localhost:8000/admin/`](http://localhost:8000/admin/) in your browser and create an author and some articles.
-        
-        ## How to test your actions?
-        
-        There are two ways on how to write tests for your actions.
-        We will use [pytest](https://docs.pytest.org/en/latest/) for the following examples.
-        
-        ### Test the action itself
-        
-        Before we can call our action on the admin class itself, we have to instantiate the admin environment and pass it to the `ModelAdmin` together with an instance of our model.
-        Therefore, we implement a fixture called `admin_site`, which is used on each test.
-        
-        ```python
-        import pytest
-        from django.contrib.admin import AdminSite
-        
-        from yourapp.module.admin import MyAdmin
-        
-        
-        @pytest.fixture
-        def admin_site():
-            return AdminSite()
-        
-        @pytest.mark.django_db
-        def test_action_XXX(admin_site):
-            """Test action XXX"""
-            fake_request = {}  # you might need to use a RequestFactory here
-            obj = ...  # create an instance
-        
-            admin = MyAdmin(obj, admin_site)
-        
-            admin.render_inline_actions(article)
-            response = admin.action_XXX(fake_request, obj)
-            # assert the state of the application
-        ```
-        
-        ### Test the admin integration
-        
-        Alternatively, you can test your actions on the real Django admin page.
-        You will have to log in, navigate to the corresponding admin and trigger a click on the action.
-        To simplify this process you can use [django-webtest](https://github.com/django-webtest/django-webtest).
-        Example can be found [here](https://github.com/HiroshiFuu/django4-inline-actions/blob/master/test_proj/blog/tests/test_inline_admin.py#L146).
-        
-        ## Development
-        
-        This project uses [poetry](https://poetry.eustace.io/) for packaging and
-        managing all dependencies and [pre-commit](https://pre-commit.com/) to run
-        [flake8](http://flake8.pycqa.org/), [isort](https://pycqa.github.io/isort/),
-        [mypy](http://mypy-lang.org/) and [black](https://github.com/python/black).
-        
-        Additionally, [pdbpp](https://github.com/pdbpp/pdbpp) and [better-exceptions](https://github.com/qix-/better-exceptions) are installed to provide a better debugging experience.
-        To enable `better-exceptions` you have to run `export BETTER_EXCEPTIONS=1` in your current session/terminal.
-        
-        Clone this repository and run
-        
-        ```bash
-        poetry install
-        poetry run pre-commit install
-        ```
-        
-        to create a virtual enviroment containing all dependencies.
-        Afterwards, You can run the test suite using
-        
-        ```bash
-        poetry run pytest
-        ```
-        
-        This repository follows the [Conventional Commits](https://www.conventionalcommits.org/)
-        style.
-        
-        ### Cookiecutter template
-        
-        This project was created using [cruft](https://github.com/cruft/cruft) and the
-        [cookiecutter-pyproject](https://github.com/escaped/cookiecutter-pypackage) template.
-        In order to update this repository to the latest template version run
-        
-        ```sh
-        cruft update
-        ```
-        
-        in the root of this repository.
-        
 Keywords: ModelAdmin inline actions
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# django4-inline-actions
+
+![PyPI](https://img.shields.io/pypi/v/django4-inline-actions?style=flat-square)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django4-inline-actions?style=flat-square)
+![PyPI - License](https://img.shields.io/pypi/l/django4-inline-actions?style=flat-square)
+<!-- ![GitHub Workflow Status (master)](https://img.shields.io/github/workflow/status/HiroshiFuu/django4-inline-actions/Test%20&%20Lint/master?style=flat-square) -->
+<!-- ![Coveralls github branch](https://img.shields.io/coveralls/github/HiroshiFuu/django4-inline-actions/master?style=flat-square) -->
+
+django4-inline-actions adds actions to each row of the ModelAdmin or InlineModelAdmin. Add support for Django 4.
+
+## Requirements
+
+* Python 3.8 or newer
+
+## Screenshot
+
+![Changelist example](https://raw.githubusercontent.com/HiroshiFuu/django4-inline-actions/master/example_changelist.png)
+![Inline example](https://raw.githubusercontent.com/HiroshiFuu/django4-inline-actions/master/example_inline.png)
+
+## Installation
+
+1. Install django4-inline-actions
+
+   ```sh
+   pip install django4-inline-actions
+   ```
+
+2. Add `inline_actions` to your `INSTALLED_APPS`.
+
+## Integration
+
+Add the `InlineActionsModelAdminMixin` to your `ModelAdmin`.
+If you want to have actions on your inlines, add the `InlineActionsMixin` to your `InlineModelAdmin`.
+Each action is implemented as a method on the `ModelAdmin`/`InlineModelAdmin` and **must have** the following signature.
+
+```python
+def action_name(self, request, obj, parent_obj=None):
+```
+
+| Argument     | Description                                       |
+|--------------|---------------------------------------------------|
+| `request`    | current request                                   |
+| `obj`        | instance on which the action was triggered        |
+| `parent_obj` | instance of the parent model, only set on inlines |
+
+and should return `None` to return to the current changeform or a `HttpResponse`.
+Finally, add your method name to list of actions `inline_actions` defined on the corresponding `ModelAdmin`.
+If you want to disable the *actions* column, you have to explicitly set `inline_actions = None`.
+To add your actions dynamically, you can use the method `get_inline_actions(self, request, obj=None)` instead.
+
+This module is bundled with two actions for viewing (`inline_actions.actions.ViewAction`) and deleting (`inline_actions.actions.DeleteAction`).
+Just add these classes to your admin and you're done.
+
+Additionally, you can add methods to generate a custom label and CSS classes per object.
+If you have an inline action called `action_name` then you can define
+
+```python
+def get_action_name_label(self, obj):
+    return 'some string'
+
+def get_action_name_css(self, obj):
+    return 'some string'
+```
+
+| Argument | Description                                |
+|----------|--------------------------------------------|
+| `obj`    | instance on which the action was triggered |
+
+Each defined method has to return a string.
+
+### Example 1
+
+Imagine a simple news application with the following `admin.py`.
+
+```python
+from django.contrib import admin
+from inline_actions.admin import InlineActionsMixin
+from inline_actions.admin import InlineActionsModelAdminMixin
+
+from .models import Article, Author
+
+
+class ArticleInline(InlineActionsMixin,
+                    admin.TabularInline):
+    model = Article
+    inline_actions = []
+
+    def has_add_permission(self, request, obj=None):
+        return False
+
+
+@admin.register(Author)
+class AuthorAdmin(InlineActionsModelAdminMixin,
+                  admin.ModelAdmin):
+    inlines = [ArticleInline]
+    list_display = ('name',)
+
+
+@admin.register(Article)
+class AuthorAdmin(admin.ModelAdmin):
+    list_display = ('title', 'status', 'author')
+```
+
+We now want to add two simple actions (`view`, `unpublish`) to each article within the `AuthorAdmin`.
+The `view` action redirects to the changeform of the selected instance.
+
+```python
+from django.core.urlresolvers import reverse
+from django.shortcuts import redirect
+
+
+class ArticleInline(InlineActionsMixin,
+                    admin.TabularInline):
+    # ...
+    inline_actions = ['view']
+    # ...
+
+    def view(self, request, obj, parent_obj=None):
+        url = reverse(
+            'admin:{}_{}_change'.format(
+                obj._meta.app_label,
+                obj._meta.model_name,
+            ),
+            args=(obj.pk,)
+        )
+        return redirect(url)
+    view.short_description = _("View")
+```
+
+Since `unpublish` depends on `article.status` we must use `get_inline_actions` to add this action dynamically.
+
+```python
+from django.contrib import admin, messages
+from django.utils.translation import gettext_lazy as _
+
+
+class ArticleInline(InlineActionsMixin,
+                    admin.TabularInline):
+    # ...
+    def get_inline_actions(self, request, obj=None):
+        actions = super(ArticleInline, self).get_inline_actions(request, obj)
+        if obj:
+            if obj.status == Article.PUBLISHED:
+                actions.append('unpublish')
+        return actions
+
+    def unpublish(self, request, obj, parent_obj=None):
+        obj.status = Article.DRAFT
+        obj.save()
+        messages.info(request, _("Article unpublished"))
+    unpublish.short_description = _("Unpublish")
+```
+
+Adding `inline_actions` to the changelist works similar. See the sample project for further details (`test_proj/blog/admin.py`).
+
+### Example 2
+
+Instead of creating separate actions for publishing and unpublishing, we might prefer an action, which toggles between those two states.
+`toggle_publish` implements the behaviour described above.
+
+```python
+def toggle_publish(self, request, obj, parent_obj=None):
+    if obj.status == Article.DRAFT:
+        obj.status = Article.PUBLISHED
+    else:
+        obj.status = Article.DRAFT
+
+    obj.save()
+
+    if obj.status == Article.DRAFT:
+        messages.info(request, _("Article unpublished."))
+    else:
+        messages.info(request, _("Article published."))
+```
+
+This might leave the user with an ambiguous button label as it will be called `Toggle publish` regardless of the internal state.
+We can specify a dynamic label by adding a special method `get_ACTIONNAME_label`.
+
+```python
+def get_toggle_publish_label(self, obj):
+    if obj.status == Article.DRAFT:
+        return 'Publish'
+    return 'Unpublish'
+```
+
+So assuming an object in a row has `DRAFT` status, then the button label will be `Toggle publish` and `Toggle unpublish` otherwise.
+
+We can go even fancier when we create a method that will add css classes for each object depending on a status like:
+
+```python
+def get_toggle_publish_css(self, obj):
+    if obj.status == Article.DRAFT:
+        return 'btn-red'
+    return 'btn-green'
+```
+
+You can make it more eye-candy by using `btn-green` that makes your button green and `btn-red` that makes your button red.
+Or you can use those classes to add some javascript logic (i.e. confirmation box).
+
+### Tip on confirmation alerts
+
+When performing a certain critical action or ones which may not be easily reversible it's good to have a confirmation prompt before submitting the action form. To achieve this, one way would be to override `templates/admin/change_list.html` with the following.
+
+```html
+{% extends "admin/change_list.html" %}
+
+{% block extrahead %}
+    {{ block.super }}
+    <script>
+        (function() {
+            document.addEventListener("DOMContentLoaded", function(event) {
+                let inline_actions = document.querySelectorAll(".inline_actions input");
+                for (var i=0; i < inline_actions.length; i++) {
+                    inline_actions[i].addEventListener("click", function(e) {
+                        if(!confirm("Do you really want to " + e.target.value + "?")) {
+                            e.preventDefault();
+                        }
+                    });
+                }
+            });
+        })();
+    </script>
+{% endblock %}
+```
+
+If a staff user has clicked any inline action accidentally, they can safely click no in the confirmation prompt & the inline action form would not be submitted.
+
+## Intermediate forms
+
+The current implementation for using intermediate forms involves some manual handling.
+This will be simplified in the next major release!
+
+
+In order to have an intermediate form, you must add some information about the triggered action.
+`django4-inline-actions` provides a handy templatetag `render_inline_action_fields`,
+which adds these information as hidden fields to a form.
+
+```html
+{% extends "admin/base_site.html" %}
+{% load inline_action_tags %}
+
+{% block content %}
+  <form action="" method="post">
+    {% csrf_token %}
+    {% render_inline_action_fields %}
+
+    {{ form.as_p }}
+
+    <input type="submit" name="_back" value="Cancel"/>
+    <input type="submit" name="_save" value="Update"/>
+  </form>
+{% endblock %}
+```
+
+As the action does not know that an intermediate form is used, we have to include some special handling.
+In the case above we have to consider 3 cases:
+
+1. The form has been submitted and we want to redirect to the previous view.
+2. Back button has been clicked.
+3. Initial access to the intermediate page/form.
+
+The corresponding action could look like
+
+```python
+    def change_title(self, request, obj, parent_obj=None):
+
+        # 1. has the form been submitted?
+        if '_save' in request.POST:
+            form = forms.ChangeTitleForm(request.POST, instance=obj)
+            form.save()
+            return None  # return back to list view
+        # 2. has the back button been pressed?
+        elif '_back' in request.POST:
+            return None  # return back to list view
+        # 3. simply display the form
+        else:
+            form = forms.ChangeTitleForm(instance=obj)
+
+        return render(
+            request,
+            'change_title.html',
+            context={'form': form}
+        )
+```
+
+## Example Application
+
+You can see `django4-inline-actions` in action using the bundled test application `test_proj`.
+Use [`poetry`](https://poetry.eustace.io/) to run it.
+
+```bash
+git clone https://github.com/HiroshiFuu/django4-inline-actions.git
+cd django4-inline-actions/
+poetry install
+poetry run pip install Django
+cd test_proj
+poetry run ./manage.py migrate
+poetry run ./manage.py createsuperuser
+poetry run ./manage.py runserver
+```
+
+Open [`http://localhost:8000/admin/`](http://localhost:8000/admin/) in your browser and create an author and some articles.
+
+## How to test your actions?
+
+There are two ways on how to write tests for your actions.
+We will use [pytest](https://docs.pytest.org/en/latest/) for the following examples.
+
+### Test the action itself
+
+Before we can call our action on the admin class itself, we have to instantiate the admin environment and pass it to the `ModelAdmin` together with an instance of our model.
+Therefore, we implement a fixture called `admin_site`, which is used on each test.
+
+```python
+import pytest
+from django.contrib.admin import AdminSite
+
+from yourapp.module.admin import MyAdmin
+
+
+@pytest.fixture
+def admin_site():
+    return AdminSite()
+
+@pytest.mark.django_db
+def test_action_XXX(admin_site):
+    """Test action XXX"""
+    fake_request = {}  # you might need to use a RequestFactory here
+    obj = ...  # create an instance
+
+    admin = MyAdmin(obj, admin_site)
+
+    admin.render_inline_actions(article)
+    response = admin.action_XXX(fake_request, obj)
+    # assert the state of the application
+```
+
+### Test the admin integration
+
+Alternatively, you can test your actions on the real Django admin page.
+You will have to log in, navigate to the corresponding admin and trigger a click on the action.
+To simplify this process you can use [django-webtest](https://github.com/django-webtest/django-webtest).
+Example can be found [here](https://github.com/HiroshiFuu/django4-inline-actions/blob/master/test_proj/blog/tests/test_inline_admin.py#L146).
+
+## Development
+
+This project uses [poetry](https://poetry.eustace.io/) for packaging and
+managing all dependencies and [pre-commit](https://pre-commit.com/) to run
+[flake8](http://flake8.pycqa.org/), [isort](https://pycqa.github.io/isort/),
+[mypy](http://mypy-lang.org/) and [black](https://github.com/python/black).
+
+Additionally, [pdbpp](https://github.com/pdbpp/pdbpp) and [better-exceptions](https://github.com/qix-/better-exceptions) are installed to provide a better debugging experience.
+To enable `better-exceptions` you have to run `export BETTER_EXCEPTIONS=1` in your current session/terminal.
+
+Clone this repository and run
+
+```bash
+poetry install
+poetry run pre-commit install
+```
+
+to create a virtual enviroment containing all dependencies.
+Afterwards, You can run the test suite using
+
+```bash
+poetry run pytest
+```
+
+This repository follows the [Conventional Commits](https://www.conventionalcommits.org/) style.
+
+## Deployment
+
+Use `setup.py` to build and upload to PyPI using `twine`.
+
+### Cookiecutter template
+
+This project was created using [cruft](https://github.com/cruft/cruft) and the
+[cookiecutter-pyproject](https://github.com/escaped/cookiecutter-pypackage) template.
+In order to update this repository to the latest template version run
+
+```sh
+cruft update
+```
+
+in the root of this repository.
```

### Comparing `django4-inline-actions-1.2/README.md` & `django4-inline-actions-1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # django4-inline-actions
 
 ![PyPI](https://img.shields.io/pypi/v/django4-inline-actions?style=flat-square)
-<!-- ![GitHub Workflow Status (master)](https://img.shields.io/github/workflow/status/HiroshiFuu/django4-inline-actions/Test%20&%20Lint/master?style=flat-square) -->
-<!-- ![Coveralls github branch](https://img.shields.io/coveralls/github/HiroshiFuu/django4-inline-actions/master?style=flat-square) -->
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django4-inline-actions?style=flat-square)
 ![PyPI - License](https://img.shields.io/pypi/l/django4-inline-actions?style=flat-square)
+<!-- ![GitHub Workflow Status (master)](https://img.shields.io/github/workflow/status/HiroshiFuu/django4-inline-actions/Test%20&%20Lint/master?style=flat-square) -->
+<!-- ![Coveralls github branch](https://img.shields.io/coveralls/github/HiroshiFuu/django4-inline-actions/master?style=flat-square) -->
 
 django4-inline-actions adds actions to each row of the ModelAdmin or InlineModelAdmin. Add support for Django 4.
 
 ## Requirements
 
 * Python 3.8 or newer
 
@@ -362,16 +362,19 @@
 to create a virtual enviroment containing all dependencies.
 Afterwards, You can run the test suite using
 
 ```bash
 poetry run pytest
 ```
 
-This repository follows the [Conventional Commits](https://www.conventionalcommits.org/)
-style.
+This repository follows the [Conventional Commits](https://www.conventionalcommits.org/) style.
+
+## Deployment
+
+Use `setup.py` to build and upload to PyPI using `twine`.
 
 ### Cookiecutter template
 
 This project was created using [cruft](https://github.com/cruft/cruft) and the
 [cookiecutter-pyproject](https://github.com/escaped/cookiecutter-pypackage) template.
 In order to update this repository to the latest template version run
```

### Comparing `django4-inline-actions-1.2/django4_inline_actions.egg-info/PKG-INFO` & `django4-inline-actions-1.3/django4_inline_actions.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,408 +1,411 @@
 Metadata-Version: 2.1
 Name: django4-inline-actions
-Version: 1.2
+Version: 1.3
 Summary: django4-inline-actions adds actions to each row of the ModelAdmin or InlineModelAdmin
 Home-page: https://github.com/HiroshiFuu/django4-inline-actions
+Download-URL: https://pypi.python.org/pypi/django4-inline-actions
 Author: FENG Hao
 Author-email: hiroshifuu@outlook.com
 License: BSD
-Download-URL: https://pypi.python.org/pypi/django4-inline-actions
-Description: # django4-inline-actions
-        
-        ![PyPI](https://img.shields.io/pypi/v/django4-inline-actions?style=flat-square)
-        <!-- ![GitHub Workflow Status (master)](https://img.shields.io/github/workflow/status/HiroshiFuu/django4-inline-actions/Test%20&%20Lint/master?style=flat-square) -->
-        <!-- ![Coveralls github branch](https://img.shields.io/coveralls/github/HiroshiFuu/django4-inline-actions/master?style=flat-square) -->
-        ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django4-inline-actions?style=flat-square)
-        ![PyPI - License](https://img.shields.io/pypi/l/django4-inline-actions?style=flat-square)
-        
-        django4-inline-actions adds actions to each row of the ModelAdmin or InlineModelAdmin. Add support for Django 4.
-        
-        ## Requirements
-        
-        * Python 3.8 or newer
-        
-        ## Screenshot
-        
-        ![Changelist example](https://raw.githubusercontent.com/HiroshiFuu/django4-inline-actions/master/example_changelist.png)
-        ![Inline example](https://raw.githubusercontent.com/HiroshiFuu/django4-inline-actions/master/example_inline.png)
-        
-        ## Installation
-        
-        1. Install django4-inline-actions
-        
-           ```sh
-           pip install django4-inline-actions
-           ```
-        
-        2. Add `inline_actions` to your `INSTALLED_APPS`.
-        
-        ## Integration
-        
-        Add the `InlineActionsModelAdminMixin` to your `ModelAdmin`.
-        If you want to have actions on your inlines, add the `InlineActionsMixin` to your `InlineModelAdmin`.
-        Each action is implemented as a method on the `ModelAdmin`/`InlineModelAdmin` and **must have** the following signature.
-        
-        ```python
-        def action_name(self, request, obj, parent_obj=None):
-        ```
-        
-        | Argument     | Description                                       |
-        |--------------|---------------------------------------------------|
-        | `request`    | current request                                   |
-        | `obj`        | instance on which the action was triggered        |
-        | `parent_obj` | instance of the parent model, only set on inlines |
-        
-        and should return `None` to return to the current changeform or a `HttpResponse`.
-        Finally, add your method name to list of actions `inline_actions` defined on the corresponding `ModelAdmin`.
-        If you want to disable the *actions* column, you have to explicitly set `inline_actions = None`.
-        To add your actions dynamically, you can use the method `get_inline_actions(self, request, obj=None)` instead.
-        
-        This module is bundled with two actions for viewing (`inline_actions.actions.ViewAction`) and deleting (`inline_actions.actions.DeleteAction`).
-        Just add these classes to your admin and you're done.
-        
-        Additionally, you can add methods to generate a custom label and CSS classes per object.
-        If you have an inline action called `action_name` then you can define
-        
-        ```python
-        def get_action_name_label(self, obj):
-            return 'some string'
-        
-        def get_action_name_css(self, obj):
-            return 'some string'
-        ```
-        
-        | Argument | Description                                |
-        |----------|--------------------------------------------|
-        | `obj`    | instance on which the action was triggered |
-        
-        Each defined method has to return a string.
-        
-        ### Example 1
-        
-        Imagine a simple news application with the following `admin.py`.
-        
-        ```python
-        from django.contrib import admin
-        from inline_actions.admin import InlineActionsMixin
-        from inline_actions.admin import InlineActionsModelAdminMixin
-        
-        from .models import Article, Author
-        
-        
-        class ArticleInline(InlineActionsMixin,
-                            admin.TabularInline):
-            model = Article
-            inline_actions = []
-        
-            def has_add_permission(self, request, obj=None):
-                return False
-        
-        
-        @admin.register(Author)
-        class AuthorAdmin(InlineActionsModelAdminMixin,
-                          admin.ModelAdmin):
-            inlines = [ArticleInline]
-            list_display = ('name',)
-        
-        
-        @admin.register(Article)
-        class AuthorAdmin(admin.ModelAdmin):
-            list_display = ('title', 'status', 'author')
-        ```
-        
-        We now want to add two simple actions (`view`, `unpublish`) to each article within the `AuthorAdmin`.
-        The `view` action redirects to the changeform of the selected instance.
-        
-        ```python
-        from django.core.urlresolvers import reverse
-        from django.shortcuts import redirect
-        
-        
-        class ArticleInline(InlineActionsMixin,
-                            admin.TabularInline):
-            # ...
-            inline_actions = ['view']
-            # ...
-        
-            def view(self, request, obj, parent_obj=None):
-                url = reverse(
-                    'admin:{}_{}_change'.format(
-                        obj._meta.app_label,
-                        obj._meta.model_name,
-                    ),
-                    args=(obj.pk,)
-                )
-                return redirect(url)
-            view.short_description = _("View")
-        ```
-        
-        Since `unpublish` depends on `article.status` we must use `get_inline_actions` to add this action dynamically.
-        
-        ```python
-        from django.contrib import admin, messages
-        from django.utils.translation import gettext_lazy as _
-        
-        
-        class ArticleInline(InlineActionsMixin,
-                            admin.TabularInline):
-            # ...
-            def get_inline_actions(self, request, obj=None):
-                actions = super(ArticleInline, self).get_inline_actions(request, obj)
-                if obj:
-                    if obj.status == Article.PUBLISHED:
-                        actions.append('unpublish')
-                return actions
-        
-            def unpublish(self, request, obj, parent_obj=None):
-                obj.status = Article.DRAFT
-                obj.save()
-                messages.info(request, _("Article unpublished"))
-            unpublish.short_description = _("Unpublish")
-        ```
-        
-        Adding `inline_actions` to the changelist works similar. See the sample project for further details (`test_proj/blog/admin.py`).
-        
-        ### Example 2
-        
-        Instead of creating separate actions for publishing and unpublishing, we might prefer an action, which toggles between those two states.
-        `toggle_publish` implements the behaviour described above.
-        
-        ```python
-        def toggle_publish(self, request, obj, parent_obj=None):
-            if obj.status == Article.DRAFT:
-                obj.status = Article.PUBLISHED
-            else:
-                obj.status = Article.DRAFT
-        
-            obj.save()
-        
-            if obj.status == Article.DRAFT:
-                messages.info(request, _("Article unpublished."))
-            else:
-                messages.info(request, _("Article published."))
-        ```
-        
-        This might leave the user with an ambiguous button label as it will be called `Toggle publish` regardless of the internal state.
-        We can specify a dynamic label by adding a special method `get_ACTIONNAME_label`.
-        
-        ```python
-        def get_toggle_publish_label(self, obj):
-            if obj.status == Article.DRAFT:
-                return 'Publish'
-            return 'Unpublish'
-        ```
-        
-        So assuming an object in a row has `DRAFT` status, then the button label will be `Toggle publish` and `Toggle unpublish` otherwise.
-        
-        We can go even fancier when we create a method that will add css classes for each object depending on a status like:
-        
-        ```python
-        def get_toggle_publish_css(self, obj):
-            if obj.status == Article.DRAFT:
-                return 'btn-red'
-            return 'btn-green'
-        ```
-        
-        You can make it more eye-candy by using `btn-green` that makes your button green and `btn-red` that makes your button red.
-        Or you can use those classes to add some javascript logic (i.e. confirmation box).
-        
-        ### Tip on confirmation alerts
-        
-        When performing a certain critical action or ones which may not be easily reversible it's good to have a confirmation prompt before submitting the action form. To achieve this, one way would be to override `templates/admin/change_list.html` with the following.
-        
-        ```html
-        {% extends "admin/change_list.html" %}
-        
-        {% block extrahead %}
-            {{ block.super }}
-            <script>
-                (function() {
-                    document.addEventListener("DOMContentLoaded", function(event) {
-                        let inline_actions = document.querySelectorAll(".inline_actions input");
-                        for (var i=0; i < inline_actions.length; i++) {
-                            inline_actions[i].addEventListener("click", function(e) {
-                                if(!confirm("Do you really want to " + e.target.value + "?")) {
-                                    e.preventDefault();
-                                }
-                            });
-                        }
-                    });
-                })();
-            </script>
-        {% endblock %}
-        ```
-        
-        If a staff user has clicked any inline action accidentally, they can safely click no in the confirmation prompt & the inline action form would not be submitted.
-        
-        ## Intermediate forms
-        
-        The current implementation for using intermediate forms involves some manual handling.
-        This will be simplified in the next major release!
-        
-        
-        In order to have an intermediate form, you must add some information about the triggered action.
-        `django4-inline-actions` provides a handy templatetag `render_inline_action_fields`,
-        which adds these information as hidden fields to a form.
-        
-        ```html
-        {% extends "admin/base_site.html" %}
-        {% load inline_action_tags %}
-        
-        {% block content %}
-          <form action="" method="post">
-            {% csrf_token %}
-            {% render_inline_action_fields %}
-        
-            {{ form.as_p }}
-        
-            <input type="submit" name="_back" value="Cancel"/>
-            <input type="submit" name="_save" value="Update"/>
-          </form>
-        {% endblock %}
-        ```
-        
-        As the action does not know that an intermediate form is used, we have to include some special handling.
-        In the case above we have to consider 3 cases:
-        
-        1. The form has been submitted and we want to redirect to the previous view.
-        2. Back button has been clicked.
-        3. Initial access to the intermediate page/form.
-        
-        The corresponding action could look like
-        
-        ```python
-            def change_title(self, request, obj, parent_obj=None):
-        
-                # 1. has the form been submitted?
-                if '_save' in request.POST:
-                    form = forms.ChangeTitleForm(request.POST, instance=obj)
-                    form.save()
-                    return None  # return back to list view
-                # 2. has the back button been pressed?
-                elif '_back' in request.POST:
-                    return None  # return back to list view
-                # 3. simply display the form
-                else:
-                    form = forms.ChangeTitleForm(instance=obj)
-        
-                return render(
-                    request,
-                    'change_title.html',
-                    context={'form': form}
-                )
-        ```
-        
-        ## Example Application
-        
-        You can see `django4-inline-actions` in action using the bundled test application `test_proj`.
-        Use [`poetry`](https://poetry.eustace.io/) to run it.
-        
-        ```bash
-        git clone https://github.com/HiroshiFuu/django4-inline-actions.git
-        cd django4-inline-actions/
-        poetry install
-        poetry run pip install Django
-        cd test_proj
-        poetry run ./manage.py migrate
-        poetry run ./manage.py createsuperuser
-        poetry run ./manage.py runserver
-        ```
-        
-        Open [`http://localhost:8000/admin/`](http://localhost:8000/admin/) in your browser and create an author and some articles.
-        
-        ## How to test your actions?
-        
-        There are two ways on how to write tests for your actions.
-        We will use [pytest](https://docs.pytest.org/en/latest/) for the following examples.
-        
-        ### Test the action itself
-        
-        Before we can call our action on the admin class itself, we have to instantiate the admin environment and pass it to the `ModelAdmin` together with an instance of our model.
-        Therefore, we implement a fixture called `admin_site`, which is used on each test.
-        
-        ```python
-        import pytest
-        from django.contrib.admin import AdminSite
-        
-        from yourapp.module.admin import MyAdmin
-        
-        
-        @pytest.fixture
-        def admin_site():
-            return AdminSite()
-        
-        @pytest.mark.django_db
-        def test_action_XXX(admin_site):
-            """Test action XXX"""
-            fake_request = {}  # you might need to use a RequestFactory here
-            obj = ...  # create an instance
-        
-            admin = MyAdmin(obj, admin_site)
-        
-            admin.render_inline_actions(article)
-            response = admin.action_XXX(fake_request, obj)
-            # assert the state of the application
-        ```
-        
-        ### Test the admin integration
-        
-        Alternatively, you can test your actions on the real Django admin page.
-        You will have to log in, navigate to the corresponding admin and trigger a click on the action.
-        To simplify this process you can use [django-webtest](https://github.com/django-webtest/django-webtest).
-        Example can be found [here](https://github.com/HiroshiFuu/django4-inline-actions/blob/master/test_proj/blog/tests/test_inline_admin.py#L146).
-        
-        ## Development
-        
-        This project uses [poetry](https://poetry.eustace.io/) for packaging and
-        managing all dependencies and [pre-commit](https://pre-commit.com/) to run
-        [flake8](http://flake8.pycqa.org/), [isort](https://pycqa.github.io/isort/),
-        [mypy](http://mypy-lang.org/) and [black](https://github.com/python/black).
-        
-        Additionally, [pdbpp](https://github.com/pdbpp/pdbpp) and [better-exceptions](https://github.com/qix-/better-exceptions) are installed to provide a better debugging experience.
-        To enable `better-exceptions` you have to run `export BETTER_EXCEPTIONS=1` in your current session/terminal.
-        
-        Clone this repository and run
-        
-        ```bash
-        poetry install
-        poetry run pre-commit install
-        ```
-        
-        to create a virtual enviroment containing all dependencies.
-        Afterwards, You can run the test suite using
-        
-        ```bash
-        poetry run pytest
-        ```
-        
-        This repository follows the [Conventional Commits](https://www.conventionalcommits.org/)
-        style.
-        
-        ### Cookiecutter template
-        
-        This project was created using [cruft](https://github.com/cruft/cruft) and the
-        [cookiecutter-pyproject](https://github.com/escaped/cookiecutter-pypackage) template.
-        In order to update this repository to the latest template version run
-        
-        ```sh
-        cruft update
-        ```
-        
-        in the root of this repository.
-        
 Keywords: ModelAdmin inline actions
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# django4-inline-actions
+
+![PyPI](https://img.shields.io/pypi/v/django4-inline-actions?style=flat-square)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django4-inline-actions?style=flat-square)
+![PyPI - License](https://img.shields.io/pypi/l/django4-inline-actions?style=flat-square)
+<!-- ![GitHub Workflow Status (master)](https://img.shields.io/github/workflow/status/HiroshiFuu/django4-inline-actions/Test%20&%20Lint/master?style=flat-square) -->
+<!-- ![Coveralls github branch](https://img.shields.io/coveralls/github/HiroshiFuu/django4-inline-actions/master?style=flat-square) -->
+
+django4-inline-actions adds actions to each row of the ModelAdmin or InlineModelAdmin. Add support for Django 4.
+
+## Requirements
+
+* Python 3.8 or newer
+
+## Screenshot
+
+![Changelist example](https://raw.githubusercontent.com/HiroshiFuu/django4-inline-actions/master/example_changelist.png)
+![Inline example](https://raw.githubusercontent.com/HiroshiFuu/django4-inline-actions/master/example_inline.png)
+
+## Installation
+
+1. Install django4-inline-actions
+
+   ```sh
+   pip install django4-inline-actions
+   ```
+
+2. Add `inline_actions` to your `INSTALLED_APPS`.
+
+## Integration
+
+Add the `InlineActionsModelAdminMixin` to your `ModelAdmin`.
+If you want to have actions on your inlines, add the `InlineActionsMixin` to your `InlineModelAdmin`.
+Each action is implemented as a method on the `ModelAdmin`/`InlineModelAdmin` and **must have** the following signature.
+
+```python
+def action_name(self, request, obj, parent_obj=None):
+```
+
+| Argument     | Description                                       |
+|--------------|---------------------------------------------------|
+| `request`    | current request                                   |
+| `obj`        | instance on which the action was triggered        |
+| `parent_obj` | instance of the parent model, only set on inlines |
+
+and should return `None` to return to the current changeform or a `HttpResponse`.
+Finally, add your method name to list of actions `inline_actions` defined on the corresponding `ModelAdmin`.
+If you want to disable the *actions* column, you have to explicitly set `inline_actions = None`.
+To add your actions dynamically, you can use the method `get_inline_actions(self, request, obj=None)` instead.
+
+This module is bundled with two actions for viewing (`inline_actions.actions.ViewAction`) and deleting (`inline_actions.actions.DeleteAction`).
+Just add these classes to your admin and you're done.
+
+Additionally, you can add methods to generate a custom label and CSS classes per object.
+If you have an inline action called `action_name` then you can define
+
+```python
+def get_action_name_label(self, obj):
+    return 'some string'
+
+def get_action_name_css(self, obj):
+    return 'some string'
+```
+
+| Argument | Description                                |
+|----------|--------------------------------------------|
+| `obj`    | instance on which the action was triggered |
+
+Each defined method has to return a string.
+
+### Example 1
+
+Imagine a simple news application with the following `admin.py`.
+
+```python
+from django.contrib import admin
+from inline_actions.admin import InlineActionsMixin
+from inline_actions.admin import InlineActionsModelAdminMixin
+
+from .models import Article, Author
+
+
+class ArticleInline(InlineActionsMixin,
+                    admin.TabularInline):
+    model = Article
+    inline_actions = []
+
+    def has_add_permission(self, request, obj=None):
+        return False
+
+
+@admin.register(Author)
+class AuthorAdmin(InlineActionsModelAdminMixin,
+                  admin.ModelAdmin):
+    inlines = [ArticleInline]
+    list_display = ('name',)
+
+
+@admin.register(Article)
+class AuthorAdmin(admin.ModelAdmin):
+    list_display = ('title', 'status', 'author')
+```
+
+We now want to add two simple actions (`view`, `unpublish`) to each article within the `AuthorAdmin`.
+The `view` action redirects to the changeform of the selected instance.
+
+```python
+from django.core.urlresolvers import reverse
+from django.shortcuts import redirect
+
+
+class ArticleInline(InlineActionsMixin,
+                    admin.TabularInline):
+    # ...
+    inline_actions = ['view']
+    # ...
+
+    def view(self, request, obj, parent_obj=None):
+        url = reverse(
+            'admin:{}_{}_change'.format(
+                obj._meta.app_label,
+                obj._meta.model_name,
+            ),
+            args=(obj.pk,)
+        )
+        return redirect(url)
+    view.short_description = _("View")
+```
+
+Since `unpublish` depends on `article.status` we must use `get_inline_actions` to add this action dynamically.
+
+```python
+from django.contrib import admin, messages
+from django.utils.translation import gettext_lazy as _
+
+
+class ArticleInline(InlineActionsMixin,
+                    admin.TabularInline):
+    # ...
+    def get_inline_actions(self, request, obj=None):
+        actions = super(ArticleInline, self).get_inline_actions(request, obj)
+        if obj:
+            if obj.status == Article.PUBLISHED:
+                actions.append('unpublish')
+        return actions
+
+    def unpublish(self, request, obj, parent_obj=None):
+        obj.status = Article.DRAFT
+        obj.save()
+        messages.info(request, _("Article unpublished"))
+    unpublish.short_description = _("Unpublish")
+```
+
+Adding `inline_actions` to the changelist works similar. See the sample project for further details (`test_proj/blog/admin.py`).
+
+### Example 2
+
+Instead of creating separate actions for publishing and unpublishing, we might prefer an action, which toggles between those two states.
+`toggle_publish` implements the behaviour described above.
+
+```python
+def toggle_publish(self, request, obj, parent_obj=None):
+    if obj.status == Article.DRAFT:
+        obj.status = Article.PUBLISHED
+    else:
+        obj.status = Article.DRAFT
+
+    obj.save()
+
+    if obj.status == Article.DRAFT:
+        messages.info(request, _("Article unpublished."))
+    else:
+        messages.info(request, _("Article published."))
+```
+
+This might leave the user with an ambiguous button label as it will be called `Toggle publish` regardless of the internal state.
+We can specify a dynamic label by adding a special method `get_ACTIONNAME_label`.
+
+```python
+def get_toggle_publish_label(self, obj):
+    if obj.status == Article.DRAFT:
+        return 'Publish'
+    return 'Unpublish'
+```
+
+So assuming an object in a row has `DRAFT` status, then the button label will be `Toggle publish` and `Toggle unpublish` otherwise.
+
+We can go even fancier when we create a method that will add css classes for each object depending on a status like:
+
+```python
+def get_toggle_publish_css(self, obj):
+    if obj.status == Article.DRAFT:
+        return 'btn-red'
+    return 'btn-green'
+```
+
+You can make it more eye-candy by using `btn-green` that makes your button green and `btn-red` that makes your button red.
+Or you can use those classes to add some javascript logic (i.e. confirmation box).
+
+### Tip on confirmation alerts
+
+When performing a certain critical action or ones which may not be easily reversible it's good to have a confirmation prompt before submitting the action form. To achieve this, one way would be to override `templates/admin/change_list.html` with the following.
+
+```html
+{% extends "admin/change_list.html" %}
+
+{% block extrahead %}
+    {{ block.super }}
+    <script>
+        (function() {
+            document.addEventListener("DOMContentLoaded", function(event) {
+                let inline_actions = document.querySelectorAll(".inline_actions input");
+                for (var i=0; i < inline_actions.length; i++) {
+                    inline_actions[i].addEventListener("click", function(e) {
+                        if(!confirm("Do you really want to " + e.target.value + "?")) {
+                            e.preventDefault();
+                        }
+                    });
+                }
+            });
+        })();
+    </script>
+{% endblock %}
+```
+
+If a staff user has clicked any inline action accidentally, they can safely click no in the confirmation prompt & the inline action form would not be submitted.
+
+## Intermediate forms
+
+The current implementation for using intermediate forms involves some manual handling.
+This will be simplified in the next major release!
+
+
+In order to have an intermediate form, you must add some information about the triggered action.
+`django4-inline-actions` provides a handy templatetag `render_inline_action_fields`,
+which adds these information as hidden fields to a form.
+
+```html
+{% extends "admin/base_site.html" %}
+{% load inline_action_tags %}
+
+{% block content %}
+  <form action="" method="post">
+    {% csrf_token %}
+    {% render_inline_action_fields %}
+
+    {{ form.as_p }}
+
+    <input type="submit" name="_back" value="Cancel"/>
+    <input type="submit" name="_save" value="Update"/>
+  </form>
+{% endblock %}
+```
+
+As the action does not know that an intermediate form is used, we have to include some special handling.
+In the case above we have to consider 3 cases:
+
+1. The form has been submitted and we want to redirect to the previous view.
+2. Back button has been clicked.
+3. Initial access to the intermediate page/form.
+
+The corresponding action could look like
+
+```python
+    def change_title(self, request, obj, parent_obj=None):
+
+        # 1. has the form been submitted?
+        if '_save' in request.POST:
+            form = forms.ChangeTitleForm(request.POST, instance=obj)
+            form.save()
+            return None  # return back to list view
+        # 2. has the back button been pressed?
+        elif '_back' in request.POST:
+            return None  # return back to list view
+        # 3. simply display the form
+        else:
+            form = forms.ChangeTitleForm(instance=obj)
+
+        return render(
+            request,
+            'change_title.html',
+            context={'form': form}
+        )
+```
+
+## Example Application
+
+You can see `django4-inline-actions` in action using the bundled test application `test_proj`.
+Use [`poetry`](https://poetry.eustace.io/) to run it.
+
+```bash
+git clone https://github.com/HiroshiFuu/django4-inline-actions.git
+cd django4-inline-actions/
+poetry install
+poetry run pip install Django
+cd test_proj
+poetry run ./manage.py migrate
+poetry run ./manage.py createsuperuser
+poetry run ./manage.py runserver
+```
+
+Open [`http://localhost:8000/admin/`](http://localhost:8000/admin/) in your browser and create an author and some articles.
+
+## How to test your actions?
+
+There are two ways on how to write tests for your actions.
+We will use [pytest](https://docs.pytest.org/en/latest/) for the following examples.
+
+### Test the action itself
+
+Before we can call our action on the admin class itself, we have to instantiate the admin environment and pass it to the `ModelAdmin` together with an instance of our model.
+Therefore, we implement a fixture called `admin_site`, which is used on each test.
+
+```python
+import pytest
+from django.contrib.admin import AdminSite
+
+from yourapp.module.admin import MyAdmin
+
+
+@pytest.fixture
+def admin_site():
+    return AdminSite()
+
+@pytest.mark.django_db
+def test_action_XXX(admin_site):
+    """Test action XXX"""
+    fake_request = {}  # you might need to use a RequestFactory here
+    obj = ...  # create an instance
+
+    admin = MyAdmin(obj, admin_site)
+
+    admin.render_inline_actions(article)
+    response = admin.action_XXX(fake_request, obj)
+    # assert the state of the application
+```
+
+### Test the admin integration
+
+Alternatively, you can test your actions on the real Django admin page.
+You will have to log in, navigate to the corresponding admin and trigger a click on the action.
+To simplify this process you can use [django-webtest](https://github.com/django-webtest/django-webtest).
+Example can be found [here](https://github.com/HiroshiFuu/django4-inline-actions/blob/master/test_proj/blog/tests/test_inline_admin.py#L146).
+
+## Development
+
+This project uses [poetry](https://poetry.eustace.io/) for packaging and
+managing all dependencies and [pre-commit](https://pre-commit.com/) to run
+[flake8](http://flake8.pycqa.org/), [isort](https://pycqa.github.io/isort/),
+[mypy](http://mypy-lang.org/) and [black](https://github.com/python/black).
+
+Additionally, [pdbpp](https://github.com/pdbpp/pdbpp) and [better-exceptions](https://github.com/qix-/better-exceptions) are installed to provide a better debugging experience.
+To enable `better-exceptions` you have to run `export BETTER_EXCEPTIONS=1` in your current session/terminal.
+
+Clone this repository and run
+
+```bash
+poetry install
+poetry run pre-commit install
+```
+
+to create a virtual enviroment containing all dependencies.
+Afterwards, You can run the test suite using
+
+```bash
+poetry run pytest
+```
+
+This repository follows the [Conventional Commits](https://www.conventionalcommits.org/) style.
+
+## Deployment
+
+Use `setup.py` to build and upload to PyPI using `twine`.
+
+### Cookiecutter template
+
+This project was created using [cruft](https://github.com/cruft/cruft) and the
+[cookiecutter-pyproject](https://github.com/escaped/cookiecutter-pypackage) template.
+In order to update this repository to the latest template version run
+
+```sh
+cruft update
+```
+
+in the root of this repository.
```

### Comparing `django4-inline-actions-1.2/django4_inline_actions.egg-info/SOURCES.txt` & `django4-inline-actions-1.3/django4_inline_actions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django4-inline-actions-1.2/inline_actions/actions.py` & `django4-inline-actions-1.3/inline_actions/actions.py`

 * *Files identical despite different names*

### Comparing `django4-inline-actions-1.2/inline_actions/admin.py` & `django4-inline-actions-1.3/inline_actions/admin.py`

 * *Files identical despite different names*

### Comparing `django4-inline-actions-1.2/inline_actions/templatetags/inline_action_tags.py` & `django4-inline-actions-1.3/inline_actions/templatetags/inline_action_tags.py`

 * *Files identical despite different names*

### Comparing `django4-inline-actions-1.2/pyproject.toml` & `django4-inline-actions-1.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 packages = [
   { include = "inline_actions" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8, <4.0"
-django = ">=3.0, <4.2"
+django = ">=3.0, <4.3"
 
 [tool.poetry.dev-dependencies]
 autoflake = "^1.4"
 better-exceptions = "^0.3.2"
 black = "^20.8b1"
 django-webtest = "^1.9"
 flake8 = "^3.8.3"
@@ -58,15 +58,15 @@
 pytest-mock = "^3.3.1"
 tox = "^3.20.0"
 tox-gh-actions = "^1.3.0"
 
 [tool.black]
 line-length = 88
 skip-string-normalization = true
-target_version = ['py36', 'py37', 'py38']
+target_version = ['py36', 'py37', 'py38', 'py311']
 include = '\.pyi?$'
 exclude = '''
 (
   /(
       \.eggs         # exclude a few common directories in the
     | \.git          # root of the project
     | \.hg
@@ -80,8 +80,7 @@
   )/
 )
 '''
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
-
```

### Comparing `django4-inline-actions-1.2/setup.cfg` & `django4-inline-actions-1.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `django4-inline-actions-1.2/setup.py` & `django4-inline-actions-1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     REQUIRES.append('django')
 
 if sys.version_info < (3, 8):
     REQUIRES.append('python >= 3.8')
 
 
 setup(name='django4-inline-actions',
-      version=1.2,
+      version=1.3,
       description='django4-inline-actions adds actions to each row of the ModelAdmin or InlineModelAdmin',
       long_description_content_type='text/markdown',
       long_description=long_description,
       author='FENG Hao',
       author_email='hiroshifuu@outlook.com',
       url='https://github.com/HiroshiFuu/django4-inline-actions',
       download_url='https://pypi.python.org/pypi/django4-inline-actions',
```

### Comparing `django4-inline-actions-1.2/test_proj/blog/admin.py` & `django4-inline-actions-1.3/test_proj/blog/admin.py`

 * *Files identical despite different names*

### Comparing `django4-inline-actions-1.2/test_proj/blog/migrations/0001_initial.py` & `django4-inline-actions-1.3/test_proj/blog/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django4-inline-actions-1.2/test_proj/blog/models.py` & `django4-inline-actions-1.3/test_proj/blog/models.py`

 * *Files identical despite different names*

### Comparing `django4-inline-actions-1.2/test_proj/blog/tests/test_admin.py` & `django4-inline-actions-1.3/test_proj/blog/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `django4-inline-actions-1.2/test_proj/blog/tests/test_form.py` & `django4-inline-actions-1.3/test_proj/blog/tests/test_form.py`

 * *Files identical despite different names*

### Comparing `django4-inline-actions-1.2/test_proj/blog/tests/test_inline_admin.py` & `django4-inline-actions-1.3/test_proj/blog/tests/test_inline_admin.py`

 * *Files identical despite different names*

### Comparing `django4-inline-actions-1.2/test_proj/blog/tests/test_model_admin.py` & `django4-inline-actions-1.3/test_proj/blog/tests/test_model_admin.py`

 * *Files identical despite different names*

### Comparing `django4-inline-actions-1.2/test_proj/blog/tests/test_templatetags.py` & `django4-inline-actions-1.3/test_proj/blog/tests/test_templatetags.py`

 * *Files identical despite different names*

