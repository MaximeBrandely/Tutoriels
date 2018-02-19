# TUTORIELS

----------------------------------------

![matrix](http://www.lepoint.fr/images/2017/10/27/10978762lpw-10979123-article-jpg_4669854.jpg)

## Créer un formulaire de signup avec Devise :

1) Créer app rails + Gemfile Felix

2) Enlever le # de la gem devis dans le Gemfile => "bundle install"

3) Rails g devise:install

4) rails g controller Home index

5) "root 'home#index' " dans routes.rb

6) Rails g devise User

7) Rake db:migrate

8) Dans home/index insérer : 

<ul> 
	<% if user_signed_in? %> 

	<li>
		<%= link_to "Sign Out", destroy_moussaillon_session_path, method: :delete %>
	</li>


	<% else %>
	

<p>Tu n'es pas connecté il faut d'abord que tu te connectes ou t'inscrives !</p>

	<li>
		<%= link_to "Sign in", new_user_session_path %>
	</li>


	<li>
		<%= link_to "Sign up", new_user_registration_path %>
	</li>

	<% end %> 

</ul> 

9)






![Koy](https://image.noelshack.com/fichiers/2018/05/4/1517512365-koyote.png)
 **Koyote** ![Koy](https://image.noelshack.com/fichiers/2018/05/4/1517512365-koyote.png)
