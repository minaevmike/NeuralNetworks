include_directories ("${PROJECT_SOURCE_DIR}/include")
add_library(NeuralNetwork STATIC NeuralNetwork.cpp Neuron.cpp NetworkFunction.cpp NeuralLink.cpp NeuronFactory.cpp trainAlgorithm.cpp)
add_library(NeuralNetworkShared SHARED NeuralNetwork.cpp Neuron.cpp NetworkFunction.cpp NeuralLink.cpp NeuronFactory.cpp trainAlgorithm.cpp)

target_link_libraries (NeuralNetwork)

