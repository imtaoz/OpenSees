#==============================================================================
# 
#        OpenSees -- Open System For Earthquake Engineering Simulation
#                Pacific Earthquake Engineering Research Center
#
#==============================================================================

target_sources(OPS_SysOfEqn
  PRIVATE 
    SparseGenColLinSOE.cpp
    SparseGenColLinSolver.cpp
    SparseGenRowLinSOE.cpp
    SparseGenRowLinSolver.cpp
    SuperLU.cpp
  PUBLIC
    SparseGenColLinSOE.h
    SparseGenColLinSolver.h
    SparseGenRowLinSOE.h
    SparseGenRowLinSolver.h
    SuperLU.h
)

target_sources(OPS_PFEM
    PRIVATE
        PFEMCompressibleLinSOE.cpp
        PFEMCompressibleSolver.cpp
        PFEMDiaLinSOE.cpp
        PFEMDiaSolver.cpp
        PFEMLinSOE.cpp
        PFEMQuasiLinSOE.cpp
        PFEMQuasiSolver.cpp
        PFEMSolver.cpp
        PFEMSolver_Laplace.cpp
        PFEMSolver_LumpM.cpp
        PFEMSolver_LumpM.cpp
        PFEMSolver_Umfpack.cpp
    PUBLIC
        PFEMCompressibleLinSOE.h
        PFEMCompressibleSolver.h
        PFEMDiaLinSOE.h
        PFEMDiaSolver.h
        PFEMLinSOE.h
        PFEMQuasiLinSOE.h
        PFEMQuasiSolver.h
        PFEMSolver.h
        PFEMSolver_Laplace.h
        PFEMSolver_LumpM.h
        PFEMSolver_LumpM.h
        PFEMSolver_Umfpack.h
)

target_include_directories(OPS_SysOfEqn PUBLIC ${CMAKE_CURRENT_LIST_DIR})

