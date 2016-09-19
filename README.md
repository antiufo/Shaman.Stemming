# Shaman.Stemming

C#, low-allocation version of Snowball stemmers.

## Usage
```csharp
using SF.Snowball.Ext;

var stemmer = new FrenchStemmer();
stemmer.SetCurrent("complètement");
stemmer.Stem();
stemmer.GetCurrent(); // "complet"
```
For performance reasons, you can also access the internal `StringBuilder` instead of using `SetCurrent`/`GetCurrent`, using `BorrowStringBuilder`.

## Supported languages
* Danish
* Dutch
* English
* Finnish
* French
* German
* Hungarian
* Italian
* Norwegian
* Portuguese
* Romanian
* Russian
* Spanish
* Swedish
* Turkish



