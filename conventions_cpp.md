# Coding Style and Conventions

## Code Tree

All the code files must be placed in a `src/` folder.
Every namespace must be placed in a new folder. The file hierarchy should
follow the namespace hierarchy.

## Files

* The header files must have the .h extension.
* The source files must have the .cpp extension.
* The template files must have the .hpp extension.

## Classes 

The classes names are in CamelCase :

* ClassName
* Class

### Interfaces

The interfaces are prefixed by a I :

* IClass
* IMyClass

## Variables

The variables are in lower CamelCase : 

* varName
* var

### Class Variables

#### Member variables 

The member variables are prefixed by `m_` :

* m\_var
* m\_varName

#### Static variables

The static variables are prefixed by `s_` :

* s\_var
* s\_varName

### Constants

The constants are in uppercase :

* VAR\_NAME

## Methods 

Methods name are in lower CamelCase : 

### Getters 

If the variable name is `m_varName`, the getter will be : `varName()`
The getters are always declared `const` and `inline`.

### Setters

If the variable name iis `m_varName`, the setter will be : `setVarName()`.
The setters are always declared `inline`.

## Enum

Enumerations follows the same conventions than classes and constants.
Use enum class instead of enum.

```
enum class MyEnum
{
	LABEL,
	LABEL2,
	LABEL3
};
```

## Namespaces

The namespaces are in lowercase letters.

## Includes

Use the right include directive depending on the context. `#include "..."` must
be used to import headers from the same module, whereas `#include <...>` must be
used to import headers from other modules.

## Braces and indentation

The indentation follows the 
[Allman
Styles](https://fr.wikipedia.org/wiki/Style_d%27indentation#Style_Allman).

An indent file is available.

## typedef and using

Prefer using instead of typedef.

## Signals

A signal name must be prefixed by `sig` :

* m_sigCanceled // classes
* sigCanceled  

## Documentation

```
/*!
 * \brief Brief description
 * 
 * Long description
 * \param param1 description param1
 * \param param2 description param2
 * \return 
 */
```

