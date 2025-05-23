# Set SOURCES variable
set(SOURCES
    solvers/gp3p.cc
    solvers/gp4ps.cc
    solvers/p1p2ll.cc
    solvers/p2p1ll.cc
    solvers/p2p2pl.cc
    solvers/p3ll.cc
    solvers/p3p.cc
    solvers/p3p_lambdatwist.cc
    solvers/p4pf.cc
    solvers/p5lp_radial.cc
    solvers/p6lp.cc
    solvers/ugp2p.cc
    solvers/ugp3ps.cc
    solvers/up1p2pl.cc
    solvers/up2p.cc
    solvers/up1p1ll.cc
    solvers/up4pl.cc
    solvers/ugp4pl.cc
    solvers/relpose_upright_3pt.cc
    solvers/relpose_upright_planar_2pt.cc
    solvers/relpose_upright_planar_3pt.cc
    solvers/relpose_8pt.cc
    solvers/relpose_5pt.cc
    solvers/relpose_7pt.cc
    solvers/gen_relpose_upright_4pt.cc
    solvers/gen_relpose_5p1pt.cc
    solvers/gen_relpose_6pt.cc
    solvers/homography_4pt.cc
    misc/qep.cc
    misc/univariate.cc
    misc/essential.cc
    misc/re3q3.cc
    misc/colmap_models.cc
    robust.cc
    robust/ransac.cc
    robust/bundle.cc
    robust/utils.cc
    robust/sampling.cc
    robust/estimators/absolute_pose.cc
    robust/estimators/relative_pose.cc
    robust/estimators/hybrid_pose.cc
    robust/estimators/homography.cc
)

# Set HEADERS_PUBLIC variable
set(HEADERS_PUBLIC
    alignment.h
    solvers/gp3p.h
    solvers/gp4ps.h
    solvers/p1p2ll.h
    solvers/p2p1ll.h
    solvers/p2p2pl.h
    solvers/p3ll.h
    solvers/p3p.h
    solvers/p3p_lambdatwist.h
    solvers/p4pf.h
    solvers/p5lp_radial.h
    solvers/p6lp.h
    solvers/ugp2p.h
    solvers/ugp3ps.h
    solvers/up1p2pl.h
    solvers/up2p.h
    solvers/up1p1ll.h
    solvers/up4pl.h
    solvers/ugp4pl.h
    solvers/relpose_upright_3pt.h
    solvers/relpose_upright_planar_2pt.h
    solvers/relpose_upright_planar_3pt.h
    solvers/relpose_8pt.h
    solvers/relpose_5pt.h
    solvers/relpose_7pt.h
    solvers/gen_relpose_upright_4pt.h
    solvers/gen_relpose_5p1pt.h
    solvers/gen_relpose_6pt.h
    solvers/homography_4pt.h
    misc/quaternion.h
    misc/colmap_models.h
    misc/qep.h
    misc/univariate.h
    misc/sturm.h
    misc/essential.h
    misc/re3q3.h
    robust.h
    types.h
    camera_pose.h
    alignment.h
    robust/ransac.h
    robust/ransac_impl.h
    robust/bundle.h
    robust/utils.h
    robust/sampling.h
    robust/lm_impl.h
    robust/jacobian_impl.h
    robust/estimators/absolute_pose.h
    robust/estimators/relative_pose.h
    robust/estimators/hybrid_pose.h
    robust/estimators/homography.h
)

# Set HEADERS_PRIVATE variable
set(HEADERS_PRIVATE )

# library configuration
include(${PROJECT_SOURCE_DIR}/cmake/LibraryConfig.cmake)

# Eigen
target_link_libraries(${LIBRARY_NAME} Eigen3::Eigen)
