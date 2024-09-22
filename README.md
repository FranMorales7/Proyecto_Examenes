<b><u>COMANDOS IMPORTANTES</u></b>
<br/>
-->composer create-project laravel/laravel [nombre]
-->ln -s [nombre]/public/ htdocs
-->php artisan make:migration create_[nombre]_table
-->php artisan make:controller [Nombre]controller --resource --model = [Nombre]
<br/>
<b><u>Añadir la ruta del controlador en routes/web.php :</u></b>
<br/>
-->use App\Http\Controllers\ExamController;
-->Route::resource('exams', ExamController::class);
<br/>

<b><u>base.blade.php</u></b>
<br/>

-->Muy importante porque es la pagina comun que se vera en el front
-->Ruta de carpetas: resources/views/layouts
<br/>
<b><u>Añadir rutas en las vistas create, edit, index</u></b>
<br/>

-->Siguen el siguiente formato: "{{route('exams.index')}}"

<b><u>@section('content') en index.blade.php</u></b>
-->Almacena el crud que se mostrara en  @yield('content') de base.blade.php

<b><u>Vídeo de ayuda</u></b>
https://www.youtube.com/watch?v=Rxz0GwUassM
