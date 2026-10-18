sources = files(
    'mainwindow.cpp',
    'generic.cpp',
    'helpform.cpp',
    'label.cpp',
    'lineedit.cpp',
    'optionsform.cpp',
    'saveform.cpp',
    'sequence_matcher.cpp',
    'textitem.cpp',
    'aboutform.cpp',
)

mocs = qt6.compile_moc(
    headers:[
        'mainwindow.hpp',
        'helpform.hpp',
        'label.hpp',
        'lineedit.hpp',
        'optionsform.hpp',
        'saveform.hpp',
        'aboutform.hpp'],
    dependencies: qt6_dep,
)