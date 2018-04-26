
node {
  try {
    stage('checkout') {
      checkout scm
    }
    stage('compile') {
      javac HelloWorld.java
    }
    stage('test') {
      java HelloWorld
    }
    stage('publish') {
      echo "uploading package..."
    }
  } finally {
    stage('cleanup') {
      echo "doing some cleanup..."
    }
  }
}
