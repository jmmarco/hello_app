# Ruby on Rails Basics
Create a new rails proejct:

- `rails new app_name`
- Open project inside Code Editor
- Edit `controllers/application_controller`
- Add the following code:

```
class ApplicationController < ActionController::Base

  def hello
    render html: "Hello, world!"
  end
  
end
```
- Modify default route file to render the `hello` method:
```
Rails.application.routes.draw do
  root 'application#hello'
end
```