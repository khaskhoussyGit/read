# JAVA Coding Standard

## Spacing Convention

 Use Android Studio default `Cmd + Alt + L` or `Ctrl + Alt + L` (To be agreed)

## Naming Convention
#### Package Name

Use All small cases

#### Class

Use `CamelCase`

#### Interface (Named, Anonymous)
- Prefix with `I` (Easier to use with auto-complete)
- When declaring an instance of a class that implements Interface. Refer to Interface rather than implemented Class.

#### Local/Member/Static variables

Do not prefix with `m_`, `s_` (as modern IDE now have auto-complete and color highlighting ability)

#### Constant

Use all caps: `CONSTANT_CASE`

#### Enumeration

Same as class: `NumberType.VALUE1`

#### Method

Should start with Verb


#### Resource ID (String, View, Dimension, Values)

Use Snake case. i.e. `R.color.colorPrimary`

#### Color
- Focus on **reusability** when in Platform
  - `R.color.white_a70`
  - `R.color.toolbar_title`
- Focus on **specificity** otherwise
  - prefix with module name
  - R.color.policy_white
  - ``<module>_<color_name>``

#### XML Layout file name

Please keep this in mind: ``	WHAT_WHERE_DESCRIPTION_SIZE ``

Ex:
- Custom View
  - `view_xxx`
  - `view_dialog_xxx`
- List Item
  - `item_`
- Layout file
  - `activity_profile`

#### Definition of Camelcase

Example: (Use the bold one)
- **XmlHttpRequest** vs. XMLHTTPRequest
- **newCustomerId** vs. newCustomerID


#### Test cases

Class name is suffixed with `xxxTest`

#### Comments
- Method documentation uses Android Studio standard
- Class documentation when is necessary

#### Semantic Convention
- try/catch block
  - Refer to Sonar (Do not catch top-level `Exception` class)
- Always use Brace
  - Even when the body is empty or only one statement
  - `if(YYY) { doX(); doY(); } else { doY(); }`
  - `if(YYY) { doX(); doY(); } else {}`
