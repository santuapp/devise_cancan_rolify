# README

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version

* System dependencies

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...


Create a User using rails console

rails c
> santu = User.new
> santu.email = "santuapp@address.com"
> santu.password = "santu1234"
> santu.save

    Add a role to the new User

> santu.add_role "admin"

    Check if the user has admin rights

> santu_ability = Ability.new(santu)
> santu_ability.can? :manage, :all
  => true


