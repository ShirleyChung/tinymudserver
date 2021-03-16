Import('env')

envTinyMudServer = env.Clone()
env.VariantDir( 'build', [ '.' ], duplicate = 0 )

#####################################################

tinyMudServer = envTinyMudServer.Program( 'tinyMudServer', Glob('build/*.cpp'))
env.Install( '#out', tinyMudServer )
env.Alias( 'install', '#out' )
