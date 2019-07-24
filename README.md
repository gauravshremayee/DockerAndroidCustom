# DockerAndroidCustom
#Build Custom Android Gradle Project

$docker run --rm -v "$PWD":/home/gradle/ -w /home/gradle/MyApp android_gradle gradle -PdisablePreDex clean


$docker run --rm -v "$PWD":/home/gradle/ -w /home/gradle/MyApp android-build:android-gradle gradle -PdisablePreDex lint


$docker run --rm -v "$PWD":/home/gradle/ -w /home/gradle/MyApp andres2014/android-build:part1 gradle -PdisablePreDex clean


#gradle lint

$docker run --rm -v "$PWD":/home/gradle/ -w /home/gradle/MyApp andres2014/android-build:part1 gradle -PdisablePreDex lint

#gradle build

$docker run --rm -v "$PWD":/home/gradle/ -w /home/gradle/MyApp andres2014/android-build:part1 gradle -PdisablePreDex assembleGoogleFlavorMyAppNameFreeArmv7aDebug

