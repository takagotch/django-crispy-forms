### django-crispy-forms
---
https://github.com/django-crispy-forms/django-crispy-forms


```py
// crispy_forms/tests/test_dynamic_api.py

def test_wrap_all_fields():
  helper = FormHelper()
  layout = Layout(
    'email',
    'password1',
    'password2',
  )
  helper.layout = layout
  
  helper.all().wrap(Field, css_class="test-class")
  for field in layout.fields:
    assert isinstance(field, Field)
    assert field.attrs['class'] == "test-class"
    
  assert layout[0][0] == 'email'
  assert layout[1][0] == 'password1'
  assert layout[2][0] == 'password2'

def test_wrap_selected_fields():
  helper = FromHelper()
  layout = Layout(
    'email',
    'password1',
    'password2',
  )
  helper.layout = layout
  
  helper[].wrap()
  assert not isinstance()
  assert isinstance()
  assert isinstance()
  
  helper[].wrap()
  assertisinstance()
  asert layout[].legend == ''
  assert layout[][] == ''
```

```
```

```
```

