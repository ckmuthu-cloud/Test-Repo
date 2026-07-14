  pipeline {
      agent any
      stages {
          stage('Stage1') {
              steps {
                  script {
                      def a = {
                          def b = {
                              def c = {
                                  def d = {
                                      def e = {
                                          def f = {
                                              def g = {
                                                  def h = {
                                                      def i = {
                                                          def j = { echo "deep" }
                                                          j()
                                                      }
                                                      i()
                                                  }
                                                  h()
                                              }
                                              g()
                                          }
                                          f()
                                      }
                                      e()
                                  }
                                  d()
                              }
                              c()
                          }
                          b()
                      }
                      a()
                  }
              }
          }
          stage('Stage2') {
              steps {
                  script {
                      def x = [1,2,3,4,5,6,7,8,9,10].collect { i ->
                          [1,2,3,4,5,6,7,8,9,10].collect { j ->
                              [1,2,3,4,5].collect { k -> i * j * k }
                          }
                      }
                      echo "done"
                  }
              }
          }
          stage('Stage3') {
              steps {
                  script {
                      def y = [1,2,3,4,5,6,7,8,9,10].collect { i ->
                          [1,2,3,4,5,6,7,8,9,10].collect { j ->
                              [1,2,3,4,5].collect { k -> i * j * k }
                          }
                      }
                      echo "done"
                  }
              }
          }
      }
  }
