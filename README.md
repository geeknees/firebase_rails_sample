# README

- create firebase project
- gitignore FirebaseAccountKey.json file
- rails c

```ruby
base_uri = 'https://<firebase-project-name>.firebaseio.com/'
firebase = Firebase::Client.new(base_uri, 'FirebaseAccountKey.json')
response = firebase.push("todos", { :name => 'Pick the milk', :priority => 1 })
response.success?
```

