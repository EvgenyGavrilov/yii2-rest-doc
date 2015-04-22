Tags
====

Model
------

Application use model's `fields()` function result to generate fields documents. Field's descriptions can be added 
by using `@restdoc-field` and `@restdoc-field-use-as` tags. First one is similar to phpDocumentator `@property` tag.
Second one is for using tag `@property` as a description of field.       

In an example below description and type of property `$name` will be used for field `name`. Also description and type
of `$age` property will be used for `person_age` field. 

```php
/**
 * @property string $name Name property description
 * @property int $age Age property description
 * @restdoc-field int $id ID
 * @restdoc-field string $title Model's title
 * @restdoc-field-use-as name $name
 * @restdoc-field-use-as age $person_age
 */
```
