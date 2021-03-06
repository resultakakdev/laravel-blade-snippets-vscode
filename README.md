# Laravel Blade Snippets

Laravel blade snippets and syntax highlight support for Visual Studio Code.

> Suggest Laravel related extension: [Laravel 5 Snippets](https://marketplace.visualstudio.com/items?itemName=onecentlin.laravel5-snippets)

## Screenshot

![Demo](https://github.com/onecentlin/laravel-blade-snippets-vscode/raw/master/images/screenshot.gif)

## Important update change (VS Code 1.15+)

Open `Preferences` -> `Settings`

Add below settings to enable Emmet for blade:

```json
"emmet.includeLanguages": {
    "blade": "html"
},
"emmet.triggerExpansionOnTab": true,
```

> p.s. Since VS Code v1.15, please update preference settings from `emmet.syntaxProfiles` to `emmet.includeLanguages`.
>
> Please set `emmet.triggerExpansionOnTab` value to `true` if you want to enable tab to expanse emmet tags.

## Features

* Blade syntax highlight
* Laravel blade snippets
* Emmet works in blade template

## Blade Syntax Hightlight

![Language Mode](https://github.com/onecentlin/laravel-blade-snippets-vscode/raw/master/images/language-mode.png)

* Auto detected with `.blade.php` extension
* Manually switch language mode to `Laravel Blade` (`Ctrl + K, M` or `⌘ + K, M`)

## Laravel Blade Snippets

| Trigger        | Snippet                         |
|----------------|---------------------------------|
| b:extends      | @extends                        |
| b:yield        | @yield                          |
| b:section      | @section...@endsection          |
| b:section-show | @section...@show                |
| b:if           | @if...@endif                    |
| b:if-else      | @if...@else...@endif            |
| b:has-section  | @hasSection...@else...@endif    |
| b:for          | @for...@endfor                  |
| b:foreach      | @foreach...@endforeach          |
| b:forelse      | @forelse...@empty...@endforelse |
| b:while        | @while...@endwhile              |
| b:each         | @each                           |
| b:push         | @push...@endpush                |
| b:stack        | @stack                          |
| b:inject       | @inject                         |
| b:comment      | {{-- comment --}}  (`Ctrl+/`)   |
| b:echo         | {{ $data }}                     |
| b:echo-html    | {!! $html !!}                   |
| b:echo-raw     | @{{ variable }}                 |
| b:can          | @can...@endcan (v5.1)           |
| b:can-elsecan  | @can...@elsecan...@endcan (v5.1)|
| b:cannot       | @cannot...@endcannot (v5.3)     |
| b:cannot-elsecannot | @cannot...@elsecannot...@endcannot (v5.3) |
| b:verbatim     | @verbatim...@endverbatim  (v5.3)|
| b:php          | @php...@endphp  (v5.3)          |
| b:includeIf    | @includeIf  (v5.3)              |
| b:component    | @component...@endcomponent (v5.4)|
| b:slot         | @slot...@endslot (v5.4)         |
| b:includeWhen  | @includeWhen (v5.4)             |
| b:isset        | @isset...@endisset (v5.4)       |
| b:empty        | @empty...@endempty (v5.4)       |
| b:auth         | @auth...@endauth (v5.5)         |
| b:guest        | @guest...@endguest (v5.5)       |
| b:switch       | @switch...@case...@endswitch (v5.5)   |

### $loop variable (Laravel v5.3+)

| Trigger        | Snippet                         |
|----------------|---------------------------------|
| b:loop         | $loop->(index,remaining,count,first,last,depth,parent) |
| b:loop-first   | @if($loop->first)...@endif      |
| b:loop-last    | @if($loop->last)...@endif       |

## Laravel Helper Snippets for Blade

| Trigger         | Laravel Helper                  |
|-----------------|---------------------------------|
| lv:elixir       | elixir()                        |
| lv:mix          | mix()  (v5.4)                   |
| lv:trans        | trans()                         |
| lv:action       | action()                        |
| lv:secure-asset | secure_asset()                  |
| lv:url          | url()                           |
| lv:asset        | asset()                         |
| lv:route        | route()                         |
| lv:csrf-field   | csrf_field()                    |
| lv:csrf-token   | csrf_token()                    |
| lv:pagination-links | $collection->links()        |

## Contact

Please file any [issues](https://github.com/onecentlin/laravel-blade-snippets-vscode/issues) or have a suggestion please tweet me [@onecentlin](https://twitter.com/onecentlin).

## Credits

* Blade language grammar is based on [Medalink syntax definition](https://github.com/Medalink/laravel-blade) for Sublime Text.
* Textmate language format file is based on [Textmate bundle for Laravel 5](https://github.com/loranger/Laravel.tmbundle).

## License

Please read [License](https://github.com/onecentlin/laravel-blade-snippets-vscode/blob/master/LICENSE.md) for more information