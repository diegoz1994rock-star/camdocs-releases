# Avisos y licencias de terceros — CAM DOCS

© 2026 ASTRIM. TODOS LOS DERECHOS RESERVADOS. Sitio web oficial: https://astrim-web.web.app/

CAM DOCS incorpora tecnologías de terceros. Estos componentes pertenecen a sus respectivos titulares, mantienen sus propias licencias y condiciones de uso, y ASTRIM no reclama su propiedad. El texto íntegro de cada licencia de los paquetes incluidos en la aplicación se puede consultar en Ajustes › Acerca de CAM DOCS › Licencias de terceros.

Este archivo se genera con `python tool/gen_notices.py` a partir de `pubspec.lock` y de los archivos LICENSE de cada paquete. El titular indicado es la primera línea de copyright del archivo LICENSE.

## Componentes nativos y de plataforma

- **Flutter** (motor y framework) — © The Flutter Authors — BSD 3-Clause. El motor de Flutter
  incluye a su vez componentes de terceros (Skia, ICU, HarfBuzz, FreeType, zlib, entre otros) cuyas
  licencias completas se muestran en la aplicación: Ajustes › Acerca de CAM DOCS › Licencias de
  terceros › Textos completos de las licencias.
- **Dart SDK** — © the Dart project authors — BSD 3-Clause.
- **OpenCV 4.13.0** (módulos core, imgproc e imgcodecs, compilados por `dartcv4`/`opencv_dart`) —
  © OpenCV team y colaboradores — Apache License 2.0. Incluye, compiladas dentro de la biblioteca
  nativa, las siguientes bibliotecas con sus propias licencias:
  - libjpeg-turbo — licencias IJG y BSD 3-Clause modificada (estilo BSD).
  - libpng — PNG Reference Library License version 2 — © The PNG Reference Library Authors.
  - libtiff — licencia libtiff (estilo BSD) — © Sam Leffler, © Silicon Graphics, Inc.
  - libwebp — BSD 3-Clause — © Google Inc.
  - OpenJPEG — BSD 2-Clause.
  - zlib 1.3.1 — zlib License — © Jean-loup Gailly y Mark Adler.
  - Carotene (HAL de OpenCV para ARM) — BSD 3-Clause — © NVIDIA Corporation.
- **Google ML Kit Text Recognition** (`com.google.mlkit:text-recognition:16.0.1`, Android) — Google
  LLC — se rige por las ML Kit Terms of Service, que incorporan las Google APIs Terms of Service
  (https://developers.google.com/ml-kit/terms). No es software de código abierto. Los modelos se
  consideran software relacionado y no pueden someterse a ingeniería inversa. ML Kit envía a Google
  métricas técnicas de uso (ver la Política de privacidad).
- **AndroidX AppCompat** (`androidx.appcompat:appcompat:1.7.1`) y demás bibliotecas AndroidX que
  incorporan los complementos (CameraX, Biometric, etc.) — The Android Open Source Project —
  Apache License 2.0.
- **Apple Vision** (iOS) — framework del sistema operativo de Apple; no se distribuye con la
  aplicación. Su uso se rige por el Apple Developer Program License Agreement.
- **Material Icons** y **Cupertino Icons** — fuentes de iconos incluidas por Flutter — Apache License
  2.0 (Google) y MIT respectivamente.

## Servicios externos (no incluidos en la aplicación)

- **Anthropic API (Claude)** — servicio en la nube opcional, usado solo con la clave de API del
  usuario y su autorización en cada envío. Se rige por las condiciones y la política de privacidad de
  Anthropic (https://www.anthropic.com/legal/privacy). CAM DOCS no incluye software de Anthropic: se
  comunica con su API mediante HTTPS.

## Paquetes Dart y Flutter usados directamente por la aplicación

- **archive** 4.7.1 — (c) 2013-2021 Brendan Duncan — MIT
- **camera** 0.12.2 — 2013 The Flutter Authors — BSD 3-Clause
- **crypto** 3.0.8 — 2015, the Dart project authors — BSD 3-Clause
- **cupertino_icons** 1.0.9 — (c) 2016 Vladimir Kharlampidi — MIT
- **file_picker** 13.3.3 — (c) 2018 Miguel Ruivo — MIT
- **flutter_riverpod** 3.5.0 — (c) 2020 Remi Rousselet — MIT
- **flutter_secure_storage** 11.2.0 — 2017 German Saprykin — BSD 3-Clause
- **go_router** 18.1.4 — 2013 The Flutter Authors — BSD 3-Clause
- **http** 1.6.0 — 2014, the Dart project authors — BSD 3-Clause
- **image_picker** 1.2.4 — 2013 The Flutter Authors — Apache License 2.0
- **intl** 0.20.3 — 2013, the Dart project authors — BSD 3-Clause
- **local_auth** 3.0.2 — 2013 The Flutter Authors — BSD 3-Clause
- **opencv_dart** 2.2.2 — ver LICENSE del paquete — Apache License 2.0
- **path** 1.9.1 — 2014, the Dart project authors — BSD 3-Clause
- **path_provider** 2.1.6 — 2013 The Flutter Authors — BSD 3-Clause
- **pdf** 3.13.1 — ver LICENSE del paquete — Apache License 2.0
- **pointycastle** 4.0.0 — (c) 2000 - 2019 The Legion of the Bouncy Castle Inc. (https://www.bouncycastle.org) — MIT
- **share_plus** 13.3.1 — 2017, the Flutter project authors. All rights reserved — BSD 3-Clause
- **shared_preferences** 2.5.6 — 2013 The Flutter Authors — BSD 3-Clause
- **sqflite** 2.4.6 — (c) 2019, Alexandre Roux Tekartik — BSD 2-Clause
- **url_launcher** 6.3.2 — 2013 The Flutter Authors. All rights reserved — BSD 3-Clause
- **uuid** 4.6.0 — (c) 2021 Yulian Kuncheff — MIT

## Paquetes Dart y Flutter transitivos

Dependencias de los paquetes anteriores resueltas en `pubspec.lock`. Algunas solo se usan en otras plataformas, al compilar o en las pruebas y no se incluyen en la aplicación instalada.

- **android_file_picker** 2.1.6 — (c) 2018 Miguel Ruivo — MIT
- **args** 2.7.0 — 2013, the Dart project authors — BSD 3-Clause
- **async** 2.13.1 — 2015, the Dart project authors — BSD 3-Clause
- **barcode** 2.2.9 — ver LICENSE del paquete — Apache License 2.0
- **bidi** 2.0.13 — (c) 2020 Mahdi K. Fard — MIT
- **boolean_selector** 2.1.2 — 2016, the Dart project authors — BSD 3-Clause
- **camera_android_camerax** 0.7.6+1 — 2013 The Flutter Authors — BSD 3-Clause
- **camera_avfoundation** 0.11.1 — 2013 The Flutter Authors — BSD 3-Clause
- **camera_platform_interface** 2.15.0 — 2013 The Flutter Authors — BSD 3-Clause
- **camera_web** 0.3.6 — 2013 The Flutter Authors — BSD 3-Clause
- **change_case** 2.2.0 — (c) 2021 Very Good Ventures — MIT
- **characters** 1.4.1 — 2019, the Dart project authors — BSD 3-Clause
- **clock** 1.1.3 — ver LICENSE del paquete — Apache License 2.0
- **code_assets** 1.2.1 — 2025, the Dart project authors — BSD 3-Clause
- **collection** 1.19.1 — 2015, the Dart project authors — BSD 3-Clause
- **convert** 3.1.2 — 2015, the Dart project authors — BSD 3-Clause
- **cross_file** 0.3.5+5 — 2013 The Flutter Authors — BSD 3-Clause
- **cupertino_ui** 1.1.6 — 2013 The Flutter Authors — BSD 3-Clause
- **dartcv4** 2.2.2 — ver LICENSE del paquete — Apache License 2.0
- **dbus** 0.8.0 — ver LICENSE del paquete — Mozilla Public License 2.0
- **fake_async** 1.3.3 — ver LICENSE del paquete — Apache License 2.0
- **ffi** 2.2.0 — 2019, the Dart project authors — BSD 3-Clause
- **ffi_leak_tracker** 0.1.2 — (c) 2026, Halil Durmus — BSD 3-Clause
- **file** 7.0.1 — 2017, the Dart project authors. All rights reserved — BSD 3-Clause
- **file_picker_darwin** 2.5.1 — (c) 2018 Miguel Ruivo — MIT
- **file_picker_linux** 2.0.4 — (c) 2018 Miguel Ruivo — MIT
- **file_picker_platform_interface** 4.2.0 — (c) 2018 Miguel Ruivo — MIT
- **file_picker_web** 4.2.1 — (c) 2018 Miguel Ruivo — MIT
- **file_selector_linux** 0.9.4+1 — 2013 The Flutter Authors — BSD 3-Clause
- **file_selector_macos** 0.9.5+2 — 2013 The Flutter Authors — BSD 3-Clause
- **file_selector_platform_interface** 2.7.0 — 2013 The Flutter Authors — BSD 3-Clause
- **file_selector_windows** 0.9.3+6 — 2013 The Flutter Authors — BSD 3-Clause
- **fixnum** 1.1.1 — 2014, the Dart project authors — BSD 3-Clause
- **flutter_plugin_android_lifecycle** 2.0.35 — 2013 The Flutter Authors — BSD 3-Clause
- **flutter_secure_storage_darwin** 0.4.3 — 2025 Julian Steenbakker — BSD 3-Clause
- **flutter_secure_storage_linux** 3.0.3 — 2017 German Saprykin — BSD 3-Clause
- **flutter_secure_storage_platform_interface** 2.1.1 — 2017 German Saprykin — BSD 3-Clause
- **flutter_secure_storage_web** 2.1.1 — 2017 German Saprykin — BSD 3-Clause
- **flutter_secure_storage_windows** 4.2.2 — 2017 German Saprykin — BSD 3-Clause
- **glob** 2.2.0 — 2014, the Dart project authors — BSD 3-Clause
- **hooks** 2.0.2 — 2025, the Dart project authors — BSD 3-Clause
- **http_parser** 4.1.2 — 2014, the Dart project authors — BSD 3-Clause
- **image_picker_android** 0.8.13+25 — 2013 The Flutter Authors — Apache License 2.0
- **image_picker_for_web** 3.1.1 — 2013 The Flutter Authors — BSD 3-Clause
- **image_picker_ios** 0.8.13+15 — 2013 The Flutter Authors — Apache License 2.0
- **image_picker_linux** 0.2.2 — 2013 The Flutter Authors. All rights reserved — BSD 3-Clause
- **image_picker_macos** 0.2.2+1 — 2013 The Flutter Authors — BSD 3-Clause
- **image_picker_platform_interface** 2.11.2 — 2013 The Flutter Authors — BSD 3-Clause
- **image_picker_windows** 0.2.2 — 2013 The Flutter Authors. All rights reserved — BSD 3-Clause
- **jni** 1.1.2 — 2022, the Dart project authors — BSD 3-Clause
- **jni_flutter** 1.0.4+1 — 2026, the Dart project authors — BSD 3-Clause
- **jni_util** 1.0.0 — 2026, the Dart project authors — BSD 3-Clause
- **leak_tracker** 11.0.2 — 2022, the Dart project authors — BSD 3-Clause
- **leak_tracker_flutter_testing** 3.0.10 — 2022, the Dart project authors — BSD 3-Clause
- **leak_tracker_testing** 3.0.2 — 2022, the Dart project authors — BSD 3-Clause
- **lints** 6.1.0 — 2021, the Dart project authors — BSD 3-Clause
- **listen** 1.0.1 — 2013 The Flutter Authors — BSD 3-Clause
- **local_auth_android** 2.3.0 — 2013 The Flutter Authors — BSD 3-Clause
- **local_auth_darwin** 2.0.5 — 2013 The Flutter Authors — BSD 3-Clause
- **local_auth_platform_interface** 1.1.0 — 2013 The Flutter Authors — BSD 3-Clause
- **local_auth_windows** 2.0.2 — 2013 The Flutter Authors — BSD 3-Clause
- **logging** 1.3.0 — 2013, the Dart project authors — BSD 3-Clause
- **matcher** 0.12.20 — 2014, the Dart project authors — BSD 3-Clause
- **material_color_utilities** 0.13.0 — 2021 Google LLC — Apache License 2.0
- **material_ui** 1.11.0 — 2013 The Flutter Authors — BSD 3-Clause
- **meta** 1.18.3 — 2016, the Dart project authors — BSD 3-Clause
- **mime** 2.1.0 — 2015, the Dart project authors — BSD 3-Clause
- **native_toolchain_c** 0.19.2 — 2023, the Dart project authors — BSD 3-Clause
- **native_toolchain_cmake** 0.3.2 — ver LICENSE del paquete — Apache License 2.0
- **objective_c** 9.5.0 — 2024, the Dart project authors — BSD 3-Clause
- **package_config** 3.0.0 — 2019, the Dart project authors — BSD 3-Clause
- **path_parsing** 1.1.0 — (c) 2018 Dan Field — MIT
- **path_provider_android** 2.3.1 — 2013 The Flutter Authors — BSD 3-Clause
- **path_provider_foundation** 2.6.0 — 2013 The Flutter Authors — BSD 3-Clause
- **path_provider_linux** 2.2.2 — 2013 The Flutter Authors — BSD 3-Clause
- **path_provider_platform_interface** 2.1.3 — 2013 The Flutter Authors — BSD 3-Clause
- **path_provider_windows** 2.3.0 — 2013 The Flutter Authors. All rights reserved — BSD 3-Clause
- **petitparser** 7.0.2 — (c) 2006-2024 Lukas Renggli — MIT
- **platform** 3.2.0 — 2017, the Dart project authors. All rights reserved — BSD 3-Clause
- **plugin_platform_interface** 2.1.8 — 2013 The Flutter Authors. All rights reserved — BSD 3-Clause
- **posix** 6.5.4 — (c) 2020 Brett Sutton — MIT
- **pub_semver** 2.2.1 — 2014, the Dart project authors — BSD 3-Clause
- **qr** 3.0.3 — 2014, the Dart QR project authors. All rights reserved — BSD 3-Clause
- **record_use** 0.6.0 — 2024, the Dart project authors — BSD 3-Clause
- **riverpod** 3.5.0 — (c) 2020 Remi Rousselet — MIT
- **share_plus_platform_interface** 7.2.0 — 2017 The Chromium Authors. All rights reserved — BSD 3-Clause
- **shared_preferences_android** 2.5.5 — 2013 The Flutter Authors — BSD 3-Clause
- **shared_preferences_foundation** 2.5.7 — 2013 The Flutter Authors — BSD 3-Clause
- **shared_preferences_linux** 2.4.1 — 2013 The Flutter Authors. All rights reserved — BSD 3-Clause
- **shared_preferences_platform_interface** 2.4.2 — 2013 The Flutter Authors — BSD 3-Clause
- **shared_preferences_web** 2.4.3 — 2013 The Flutter Authors. All rights reserved — BSD 3-Clause
- **shared_preferences_windows** 2.4.1 — 2013 The Flutter Authors. All rights reserved — BSD 3-Clause
- **source_span** 1.10.2 — 2014, the Dart project authors — BSD 3-Clause
- **sqflite_android** 2.4.6 — (c) 2019, Alexandre Roux Tekartik — BSD 2-Clause
- **sqflite_common** 2.5.17 — (c) 2019, Alexandre Roux Tekartik — BSD 2-Clause
- **sqflite_darwin** 2.4.6 — (c) 2019, Alexandre Roux Tekartik — BSD 2-Clause
- **sqflite_platform_interface** 2.4.4 — (c) 2019, Alexandre Roux Tekartik — BSD 2-Clause
- **sqlite3** 3.5.2 — (c) 2020 Simon Binder — MIT
- **stack_trace** 1.12.2 — 2014, the Dart project authors — BSD 3-Clause
- **state_notifier** 1.0.0 — (c) 2020 Remi Rousselet — MIT
- **stream_channel** 2.1.4 — 2015, the Dart project authors — BSD 3-Clause
- **stream_transform** 2.1.2 — 2017, the Dart project authors — BSD 3-Clause
- **string_scanner** 1.4.1 — 2014, the Dart project authors — BSD 3-Clause
- **synchronized** 3.6.1+1 — (c) 2016, Alexandre Roux Tekartik — MIT
- **term_glyph** 1.2.2 — 2017, the Dart project authors — BSD 3-Clause
- **test_api** 0.7.12 — 2018, the Dart project authors — BSD 3-Clause
- **typed_data** 1.4.0 — 2015, the Dart project authors — BSD 3-Clause
- **url_launcher_android** 6.3.32 — 2013 The Flutter Authors — BSD 3-Clause
- **url_launcher_ios** 6.4.1 — 2013 The Flutter Authors — BSD 3-Clause
- **url_launcher_linux** 3.2.3 — 2013 The Flutter Authors — BSD 3-Clause
- **url_launcher_macos** 3.2.5 — 2013 The Flutter Authors — BSD 3-Clause
- **url_launcher_platform_interface** 2.3.2 — 2013 The Flutter Authors. All rights reserved — BSD 3-Clause
- **url_launcher_web** 2.4.3 — 2013 The Flutter Authors — BSD 3-Clause
- **url_launcher_windows** 3.1.6 — 2013 The Flutter Authors — BSD 3-Clause
- **vector_math** 2.4.0 — 2013 The Flutter Authors — BSD 3-Clause
- **vm_service** 15.4.0 — 2015, the Dart project authors — BSD 3-Clause
- **web** 1.1.2 — 2023, the Dart project authors — BSD 3-Clause
- **win32** 6.4.0 — (c) 2024, Halil Durmus — BSD 3-Clause
- **windows_file_picker** 2.0.2 — (c) 2018 Miguel Ruivo — MIT
- **xdg_directories** 1.1.0 — 2013 The Flutter Authors. All rights reserved — BSD 3-Clause
- **xml** 7.0.1 — (c) 2006-2026 Lukas Renggli — MIT
- **yaml** 3.1.4 — (c) 2014, the Dart project authors — MIT

## Herramientas de desarrollo (no se incluyen en la aplicación)

- **flutter_lints** 6.0.0 — 2013 The Flutter Authors. All rights reserved — BSD 3-Clause
- **image** 4.12.0 — (c) 2013-2022 Brendan Duncan — MIT
- **sqflite_common_ffi** 2.4.7 — (c) 2019, Alexandre Roux Tekartik — BSD 2-Clause
