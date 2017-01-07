# How To

## Pass data to a single view:

```PHP
  return view('greeting')->with('firstname', 'Victoria');
```

or

```PHP
  return view('greeting', ['firstname' => 'Victoria']);
```

and access in the view with:

```PHP
  @if(session('firstname'))
     {{ session('firstname') }}
  @endif
```
## Pass data to all views:
See `share` method, as described in the [docs](https://laravel.com/docs/5.3/views#passing-data-to-views).
