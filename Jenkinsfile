pipeline {
      agent any
      stages {
          stage('Stage1') {
              steps {
                  script {
                      def run = { ->
                          def inner = { ->
                              def deep = { ->
                                  def deeper = { ->
                                      def deepest = { ->
                                          def a = { -> def b = { -> def c = { -> def d = { -> def e = { -> echo "deep" }; e() }; d() }; c() }; b() }; a() }
                                          deepest()
                                      }
                                      deeper()
                                  }
                                  deep()
                              }
                              inner()
                          }
                          run()
                      }
                  }
              }
          }
          stage('Stage2') { steps { script { def x = [1,2,3,4,5,6,7,8,9,10,11].collect { i -> [1,2,3,4,5].collect { j -> i * j } } } } }
          stage('Stage3') { steps { script { def x = [1,2,3,4,5,6,7,8,9,10,11].collect { i -> [1,2,3,4,5].collect { j -> i * j } } } } }
          stage('Stage4') { steps { script { def x = [1,2,3,4,5,6,7,8,9,10,11].collect { i -> [1,2,3,4,5].collect { j -> i * j } } } } }
          stage('Stage5') { steps { script { def x = [1,2,3,4,5,6,7,8,9,10,11].collect { i -> [1,2,3,4,5].collect { j -> i * j } } } } }
      }
  }
