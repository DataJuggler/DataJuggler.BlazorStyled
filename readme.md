
#News

9.13.2026: I updated this project to .NET 10. 

11.14.2024: This project has been updated to .NET 9.

# DataJuggler.BlazorStyled
This project is a fork of BlazorStyled by Chanan. The only thing I did was updgrade the project for .NET 9, 
I updated all the referenced packages and remove the tests and other items and reduced the code  down to just BlazorStyled.

# BlazorStyled

_CSS in Blazor Components_

## Docs

View the detailed [docs](https://blazorstyled.io) at https://blazorstyled.io.

## Install

dotnet add package DataJuggler.BlazorStyled --version 9.0.0

Leave off the version to install the latest.

## Why BlazorStyled?

* Maintain your css inside your component instead of a seperate file
* Eliminate all collisions - no need to use !important
* No need to worry about deploying css files - great for libraries
* css are C# strings - use variables instead of solutions like sass

### Insperation

* [Emotion](https://emotion.sh/docs/introduction)
* [Glamorous](https://glamorous.rocks/)
* [Glamor](https://github.com/threepointone/glamor)

## Short Example

```
<Styled @bind-Classname="@hover">
    label: hover-example;
    padding: 32px;
    background-color: hotpink;
    font-size: 24px;
    border-radius: 4px;
</Styled>

<Styled Classname="@hover" PseudoClass="PseudoClasses.Hover">
    color: @color;
</Styled>

<div class="@hover">
    Hover to change color.
</div>

@code {
    private string hover;
    private string color = "white";
}
```

See more in the [docs](https://chanan.github.io/BlazorStyled/) at https://chanan.github.io/BlazorStyled/.
