# ComandosAndroidStudio

### Imagem Redonda:
1.	Abrir o Gradle Scripts
2.	Abrir a Pasta build.gradle(module)
3.	Colar nas dependencies: 
	implementation 'de.hdodenhof:circleimageview:3.1.0'

4.	Dar Sing Now pra funcionar.
5.	E em vez de colocar ImagemView, colocar:
	<de.hdodenhof.circleimageview.CircleImageView


### Colocar vídeo:
1.	Abrir o Gradle Scripts
2.	Abrir a Pasta build.gradle(module)
3.	Colar nas dependencies: 
implementation 'com.pierfrancescosoffritti.androidyoutubeplayer:core:10.0.5'
4.	Dar Sing Now pra funcionar.
<com.pierfrancescosoffritti.androidyoutubeplayer.core.player.views.YouTubePlayerView
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    app:videoId="Z0hYETUR94A"
    app:autoPlay="true"
    app:showYouTubeButton="false"/>

### Desfocar Imagem:
1.	Abrir o Gradle Scripts
2.	Abrir a Pasta build.gradle(Project)
3.	Colar em allprojects, debaixo do jcenter()
	maven { url "https://jitpack.io" }
4.	Abrir a Pasta build.gradle(module)
5.	Colar nas dependencies: 
	implementation 'com.github.jgabrielfreitas:BlurImageView:1.0.1'
6.	Dar Sing Now pra funcionar.
7.	E em vez de colocar ImagemView, colocar:
8.	<com.jgabrielfreitas.core.BlurImageView
    android:alpha="0.8"
    app:radius="1"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:src="@drawable/music"
    android:scaleType="centerCrop"/>


### Bottom Navegation
- Tirar o espaço em branco do Action Mais (Bottom Navegation):
1.	Ir no activity_main.xml
2.	Retirar 
android:paddingTop="?attr/actionBarSize"
3.	Pronto.

- Fazer o NoActionBar funcionar:
1.	Ir no MainActivity.java
2.	Deletar a linha 26 ou comentar:
NavigationUI.setupActionBarWithNavController(this, navController, appBarConfiguration);


- Quando colocar o celular de lado, fazer o que tiver na tela rodar tb:
1.	Vai até a pasta MAndroidManifest.xml
2.	Encontra a activity que queira fazer isso.
3.	Colocar esse comando dentro dela
4.	android:screenOrientation="sensor"

ex.:
<activity android:name=".MainActivity"
    android:screenOrientation="sensor">
 
sensor = sensor do celular para inverter a tela automaticamente
landcape = deixa já como paisagem, usada principalmente em jogos, ela já deixa travada como paisagem
portrait = deixa a tela travada  na vertical, mesmo que coloque ela de lado.




