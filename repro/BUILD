scala_sources(
    name = "repro",
    dependencies = [
        # At the moment it is fine to run:
        # pants run repro:jar
        #
        # Uncomment the dependency below and again run:
        # pants run repro:jar
        #
        # and be presented with
        # Error: Could not find or load main class repro.Main
        # Caused by: java.lang.ClassNotFoundException: repro.Main
        
        # "//:google-cloud-pubsub"
    ]
)

deploy_jar(
    name = "jar",
    dependencies = [
        ":repro",
    ],
    main = "repro.Main",
)
