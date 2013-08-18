---
layout: post
title: "hello rails"
date: 2013-08-18 15:03
comments: true
categories: rails
---

### Deep in the crud
#### CRUD

##### Creat

Alternate Ayntax

	t = Tweet.new()
	t.save
	
or  
	
	Tweet.create()
	
	
##### Read

Tweet.find(1)
Tweet.find(3,4,5)
Tweet.all
Tweet.last
Tweet.where(:zomber => "ash")
###### method chaining
Tweet.where(:zomber => "ash").order(:zombie).limit(10)

##### Update

	t.attributes()
	t.save
	or
	t.update_attributes()

##### Delete
	t.destroy
	t.destroy_all  
  
### Models Tasts like chicken

	validates_presentce_of :status
	validates_numericality_of :fingers
	validates_uniqueness_of :toothmarks
	validates_confirmation_of :password
	validates_acceptance_of :zombification
	validates_length_of :password, :minimum => 3
	validates_format_of :email, :with => /regex/i
	validates_inclusion_of :age, :in => 21..99
	validates_exclusion_of :age, :in => 0..21,
				:message => "Sorry you must be over 21"
				

rails3
	
	validates :status, :presence => true,:length => { :minimum => 3 }
	
	
	
`has_many` and `belongs_to`

### View

	<% %> evaluate ruby
	<%= %> eval and print result
	
### Controller  

	
	format.html
    format.xml { render :xml => @tweet }
    format.json { render :json => @tweet }	

### route

#### Named Routes

 `match 'all' => "Tweet#index", :as => "all_tweets"`
<%= link_to "all tweets", all_tweets_path%>	
#### Redirect
`match '/undead' => redirect('/zombies')`  
`match 'all' => redirect('/tweets')`
#### Root Route

	root :to => "Tweets#index"
	
Route Parameters	

	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	